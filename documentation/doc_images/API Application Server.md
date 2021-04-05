**1. Get list of locales:**

http://crossword3.com/api/get/locales/?language_id=ru&country_id=RU&crossword_type=1 
```
Where:
    language_id - language id (optional)
    country_id - country id(optional)
    crossword_type - crossword type (0-all, 1-questions crosswords, 2-pictures crosswords)
Response:
[{
    id - locale id
    language_id - language id
    country_id - country id
    name - name (language (country))
    language - language
    country - country
}]
```

**2. Get the list of issues:**

http://crossword3.com/api/get/issues-list/?locale_id=ru_RU&last_issue_id=1&crossword_type=1
```
Where:
    locale_id - locale id
    last_issue_id - the last issue id (optional)
    crossword_type - crossword type (0-all, 1-questions crosswords, 2-pictures crosswords)
Response:
[{
    id - issue id
}]
```

**3. Get list of issue crosswords:**

http://crossword3.com/api/get/issue-crosswords-list/?issue_id=15
```
Where:
    issue_id - issue id
Response:
[{
    id - crossword id
    issue_id - issue id
    name - the name of the crossword
    width - the width of the crossword
    height - the height of the crossword
    cover - URL cover
}]
```

**4. Get issue crosswords:**

http://crossword3.com/api/get/issue-crosswords/?issue_id=15
```
Where:
    issue_id - issue id
Response:
[{
    id - crossword id
    locale_id - locale id
    is_pictures- is pictures only
    name - the name of the crossword
    width - the width of the crossword
    height - the height of the crossword
    wordsCount - words count
    imagesCount - images count
    cells [[{ - crossword cells
        x - cell coordinates in x
        y - cell coordinates in y
        isArrow - the first cell of the word (true, false)
        isLetter - word cell (true, false)
        isQuestion - the cell with the question (true, false)
        isImageQuestion - the first cell of the question-picture (true, false)
        question {
            id - question id
            word - answer
            question - question
        }
        isImage - a cell with a picture (true, false)
        image {
            width - the width of the picture
            height - the height of the picture
            src - picture (data: URL)
        }
        letter - the letter of the answer
        userLetter - user letter
        wordIndexH - horizontal word index or -1
        wordIndexV - vertically word index or -1
        arrowH - horizontal arrow id or 0
        arrowV - vertical arrow id or 0
        isLock - the cell is locked (true, false)
        endH - the end of the word horizontally (true, false)
        endV - the end of the word vertically (true, false)
    }]]
}]
```

**5. Get a crossword:**

http://crossword3.com/api/get/crossword/?crossword_id=27
```
Where:
    crossword_id - crossword id
Response:
{
    see "4. Get issue crosswords" 
}
```

**key = Ni00YTNmLT**

**6. Set best and worst question in crossword:**

http://crossword3.com/api/set/best-worst/?crossword_id=1&user_id=1&best_question_id=1&worst_question_id=2&token=6d498dd5dee8538678d80992f7f91809
```
Where:
    crossword_id - crossword id
    user_id - user id
    best_question_id - best question id
    worst_question_id - worst question id
    token (best_question_id+crossword_id+user_id+worst_question_id+key)
Response:
{
    message - message (default "ok")
}
```

**7. Set question mark:**

http://crossword3.com/api/set/mark-question/?user_id=1&question_id=1&mark=-1&token=bfa88d3ddd51b703da3b0f7a181af3da
```
Where:
    user_id - user id
    question_id - question id
    mark - mark ("1" or "-1") ("1" for good, "-1" for bad question)
    token - token (mark+question_id+user_id+key)
Response:
{
    message - message (default "ok")
}
```
