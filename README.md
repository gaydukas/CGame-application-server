Hi there :clap:

The Application Server is a part of the CGame Portal. He is a backend for crossword puzzle applications.
The CGame Portal includes two servers: Application Server and Crossword Server.

*Total schema of servers and connected services*

![Total schema of servers and connected services](/documentation/doc_images/servers_and_services-page2.png)

The Crossword server builds a crossword puzzle and sends it to the Application Server.

![1617165514978](https://user-images.githubusercontent.com/42923935/113277899-6c8c7600-930b-11eb-85b0-66e84ea90486.png)

This repository doesn't have the Crossword Server. It is intended for the Application Server.

The Application server includes:
* The storage of published crosswords
* Autherization and synchronization
* Hint log

There are the crossword  
[API](https://github.com/gaydukas/cgame-portal/blob/11db12b64f967d3306c3d06561573faf485eff65/documentation/API%20Application%20Server.md).

The end-users app will be use API. It can lools like:

![app mockup](https://user-images.githubusercontent.com/42923935/113244602-8a43e600-92df-11eb-92d5-d4a78c576cc8.png)
