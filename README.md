Hi there :clap:
# The CGame Portal
It's a backend for building of crosswords puzzle.

![1617165514978](https://user-images.githubusercontent.com/42923935/113277899-6c8c7600-930b-11eb-85b0-66e84ea90486.png)

Next, we are going to distribute to end-users the crossword puzzles through apps.

![app mockup](https://user-images.githubusercontent.com/42923935/113244602-8a43e600-92df-11eb-92d5-d4a78c576cc8.png)


There are an 
![API](https://github.com/gaydukas/cgame-portal/blob/11db12b64f967d3306c3d06561573faf485eff65/documentation/API%20Application%20Server.md).

We use the php, JavaScript, jQuery and the Yii2, Vue.js, Bootstrap 4.

**Total schema of servers and connected services**

![Total schema of servers and connected services](/documentation/doc_images/servers_and_services_page2.png)

**Design**

The interface mockups are [here](https://zpl.io/2ZJOr51). You need an invitation to Zeplin project for more functions, to contact to repository owner.

List of numbers screens (mockups) with descriptions is [here](https://docs.google.com/spreadsheets/d/1f45YQu2sqmVc2ZE71S8scbbatBz7ld6t7pGb-yX7Pxc/edit#gid=0)

**Addition resources**

[Flags of countries](https://www.countryflags.com/en/). There are the downloaded icons at Files Tab for 196 countries.

[Codes of countries](https://ru.wikipedia.org/wiki/ISO_3166-1)

[Codes of languages](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes)

**Coding convention**

The base of coding style in this project is the [PSR-2 Coding Style Guide](https://www.php-fig.org/psr/psr-2/).

In addition:

1. Constants write in capital letters through underscore

`$ANSWER_ULTIMATE_QUESTION = 42`

2. We begin the first word in a variable with a small letter, each next with a large one.

`myBestVariable`

3. File names of a class or model begin with a capital letter.
4. We write the names of resources with a small letter, under the underscore.

`button_action.png`

5. Do not write comments (maybe some exceptions :smile:).	

6. In JavaScript, the form of event handler entries:

`onTapButtonLogin, on onTouchButtonLogin, onEventNetwork.`

Those first we write “on”, then the type of event that is being monitored, then the source of the event.

7. Method names must be written, starting with the verb denoting the action that this method performs.
 
8. Do not use abbreviations.
 
9. Do not use numbers in the names of variables and methods.

10. CSS class names should be hyphenated:

`class="button-danger"`

11. Id HTML block to write under the underscore:

`id="button_danger"`

12. Do not rename existing variables, for example, if in MySQL the field is called crossword_id then in PHP it should be called $crossword_id or $crosswordId, but not $puzzle_id
 
13. Final software may differ slightly from the design if a developer found a more simple solution.
