The current project runs on two main classes. 
There are two JAR files to run.
Both are in the ./out/artifacts/ folder. 
For client jar, go to Client folder. 
For coordinator jar, go to Coordinator folder.


To start, in your CLI, type in the following:

java -jar [path directory of the coordinator JAR] 3001 4001 5001 6001 7001
The following should appear:
Server 0 is running at port 3001 at time: 2020.03.29 AD at 17:11:56 PDT
Server 1 is running at port 4001 at time: 2020.03.29 AD at 17:11:56 PDT
Server 2 is running at port 5001 at time: 2020.03.29 AD at 17:11:56 PDT
Server 3 is running at port 6001 at time: 2020.03.29 AD at 17:11:56 PDT
Server 4 is running at port 7001 at time: 2020.03.29 AD at 17:11:56 PDT


Then open up another CLI window, and type in the following:

java -jar [path directory of the client JAR] [port numbers separated by white space] [sampLe run txt file path]

For example, if the sample run txt file is ClientRequest.txt, specify it in your last argument, such as:

Java -jar 3001 4001 /Users/Sam/Desktop/project3/out/artifacts/Client/ClientRequest.txt
To switch to other sample runs (e.g., ClientRequestGetOnly.txt, ClientRequestPutOnly, ClientRequestDeleteOnly), specify as instructed.

The ClientRequest.txt sample run consists of a mix of at least five of each operation: 5 PUTs, 5 GETs, 5 DELETEs. 
