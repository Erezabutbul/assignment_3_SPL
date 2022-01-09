* In addition submit a readme.txt file that contains specifications for:
1)How to run your code
~Server:
mvn clean
mvn compile

1.1)
for TPC:
mvn exec:java -Dexec.mainClass="bgu.spl.net.impl.BGSServer.TPCMain" -Dexec.args="217"

for reactor:
mvn exec:java -Dexec.mainClass="bgu.spl.net.impl.BGSServer.ReactorMain" -Dexec.args="217 3"

1.2)
REGISTER A 1 11.11.1111
LOGIN A 1 1
PM B WHAT IS UP
POST @B how are you?
BLOCK B
STAT B
LOGSTAT

2)
we stored each set of words in each server as a private field -  vector: name -forbbidenWords

