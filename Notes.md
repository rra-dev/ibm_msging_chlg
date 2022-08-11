# NOTES - IBM MQ Badge Messaging app Challenge
Ref: [IBM MQ badge Challenge](https://developer.ibm.com/tutorials/mq-badge-mq-dev-challenge/)

[Project README](./README.md)
[GPLv2 License](./LICENSE) - Not sure why I chose this license, seemed appropriate.

## First Steps
~~Make folder, and initialize project on github~~

### ~~[Prerequisites](https://developer.ibm.com/tutorials/mq-badge-mq-dev-challenge/#Prerequisites)~~ Complete 220811
1. Java Development Kit (JDK) to develop and run applications. You need a minimum of JDK 9 installed. JDK 11 is recommended. If you don't have Java installed, go to the IBM Semeru Runtime Downloads page, select Java 11 and your platform. On some platforms, you can pull in and install it using the command line. Just make sure to get the JDK (Java Development Kit), for developing, not just the JRE (Java Runtime Environment).~~ Complete 220811

    a. Going to try with OpenJDK 17
```bash
    sudo apt install openjdk-17-jdk openjdk-17-jre
```
   
2. Sample code for this MQ Developer Challenge, in the mq-dev-badge-sample repo.~~ Complete 220811 [Code Sample README](../mq-dev-badge-sample/README.md)
    
3. [Maven](https://maven.apache.org/download.cgi) to manage all the *.jar files.~~ Complete 220811
```bash
    sudo apt install maven
```

### [The Challenge](https://developer.ibm.com/tutorials/mq-badge-mq-dev-challenge/#the-challenge)


    Connect to a queue manager (the one we provided)
    Subscribe to the newTickets topic
    Send a request message to purchase a batch of tickets, set a reply-to destination and message expiry of 15 minutes (we don’t want to commit to a purchase indefinitely)
    Get a response message from the confirmation queue specified as the reply-to destination
    Print out the result

--Checking Email and lunch