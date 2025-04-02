### Chordiflyyy

Chordify is a Peer-to-Peer song-sharing application built on the Chord Distributed Hash Table (DHT) algorithm. The project focuses on implementing distributed system features such as node management, data replication, and consistency models. The system uses SHA1 hashing to store and query songs and supports two consistency models (linearizability and eventual consistency). A command-line interface allows users to interact with the network, managing nodes and songs. 

#### Team 32
| AM      | Name                    |
|---------|-------------------------|
| el20034 | Μαρντιροσιάν Φίλιππος    |
| el20874 | Μπέλσης Παναγιώτης      |
| el20109 | Θεοδοσίου Γεώργιος      |

### CLI commands
`insert <key> <value>`

Data Insertion: A new (key, value) pair is inserted, where the key is the song title and the value is any string (which is supposed to represent the node to which we must connect to download the song). 

`delete <key>`

Data Deletion: The (key, value) pair with the given key is deleted.

`query <key>`

Data Query: The key is queried, and the corresponding value is returned from the node responsible for that key (or from a replica node). In the special case where the key is *, all <key, value> pairs stored across the entire DHT by node will be returned.

`depart`

Node Departure: The node gracefully leaves the system.

`overlay`

Network Topology Print: The nodes in the Chord ring are printed in the order in which they are connected.

`help`

Explanation of the above commands.

### Technologies Used

Python, Flask, VM's provided by AWS, Bash scripts (.sh), Linux.

![image](https://github.com/user-attachments/assets/6a03846a-bbcb-4701-b098-77492bd68af6)


### !!!ATTENTION!!!
IN ORDER TO WORK USE UBUNTU, NOT WSL!

Requirements:  
sudo apt install python3-pyfiglet  
sudo apt install python3-prettytable  
sudo apt install python3-flask  
sudo apt install python-is-python3  

