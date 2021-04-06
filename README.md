Hi there :clap:
# The CGame Portal
It's a backend for crossword puzzle applications.
The CGame Portal inclides two servers: Crossword Server and Application Server.

*Total schema of servers and connected services*

![Total schema of servers and connected services](/documentation/doc_images/servers_and_services_page2.png)

The Crossword server builds a crossword puzzle and sends it to the Application Server. This repository doesn't have the Crossword Server only the Application Server.

![1617165514978](https://user-images.githubusercontent.com/42923935/113277899-6c8c7600-930b-11eb-85b0-66e84ea90486.png)

The Application server includes:
* The storage of published crosswords
* Autherization and synchronization
* Hint log

There are an 
[API](https://github.com/gaydukas/cgame-portal/blob/11db12b64f967d3306c3d06561573faf485eff65/documentation/API%20Application%20Server.md).

Next, we are going to distribute to end-users the crossword puzzles through apps.

![app mockup](https://user-images.githubusercontent.com/42923935/113244602-8a43e600-92df-11eb-92d5-d4a78c576cc8.png)
