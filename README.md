PROJECT -3
TAPESTRY ALGORITHM - COP5615: Fall 2019

TEAM INFO
--------------------------------------------------------------------------------------------------------
Srinadh Kakkera(UFID: 0514-0863)
Neeharika Khera(UFID: 8950-0993)

PROBLEM STATEMENT
--------------------------------------------------------------------------------------------------------
Design Tapestry Algorithm using genserver/Actor model in Elixir to implement the network join and routing.

INSTALLATION AND RUN
---------------------------------------------------------------------------------------------------------
Elixir Mix project needs to be installed. The project lib folder contains the following files.

Server.ex ->The Server takes input number of nodes and no of Requests and creates n-1 Nodes for n number of nodes

createActors.ex ->Creates actors under a Supervisor 

Actor.ex -> Contains the code for actor functions

To run a test case, do:

->Unzip contents to your desired elixir project folder.
->The executable file is already created under the name of mainmodulex.
->To execute the file use the following command "./mainmodulex <<number.of.nodes>> <<number.of.requests>>
The result provides the maximum number of hops among all the hops that the nodes took to send message to their destination nodes.
Example:

PS C:\Users\srina\OneDrive\Desktop\FINAL\Proj3> escript mainmodulex 1000 10
Maximum hop value is 3


WHAT IS WORKING
--------------------------------------------------------------------------------------------------------------
Tapestry algorithm is successfully implemented. 
Step By Step Implementaion

Nodes are created(N-1)
One node is dynamically joined
While searching for prefix matching instead of 40digit hashes used in Tapestry, for our convinience and computability 40 digit hash is prefixmatched only for 8 digits
Actors start sending messages
 Each actor sends noOfReq number of Requests

and Max hop of all the requests is calculated
LARGEST NETWORK
--------------------------------------------------------------------------------------------------------------
Largest network tested:

Largest Number of Nodes tested: 2000

Largest Number of Requests: 100

Result sample:

PS C:\Users\srina\OneDrive\Desktop\FINAL\Proj3> escript mainmodulex 2000 10
Maximum hop value is 4