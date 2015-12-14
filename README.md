# java_distributedSystems
Distributed Systems project as part of my college work.

1. Dependencies

Import both of the project folders Client and Service

Using Mars eclipse

Libararies
- Apache Tomcat 8.0
- Ear Libraries
- JRE System Library [jdk 1.8.0_65]
- Web App Libaries

Make sure you have a Apache Tom Cat 8 Server
Make sure the project is JRE 1.8 compliant

2. Supplied Text for encryption

Decrypt this

UHTDUEIEJSAPSFPNUEYRMIDSUOOPNOYDURLEFWZCLIYRFNNCZPETPN

To get this

THISTEXTISPERFECTENGLISHTODEMONSTRATEWORKINGENCRYPTION

3.

Classes

-----------------------------
In Client there is 5 classes
-----------------------------

CrackerHandler - Initializes, Loads jsp page, Creates message handler, requests that stuff is decyphered

MessageHandler - Holds a thread pool, blocking inQueue and HashMap outQueue. Offers made to queue, thread does the work. checkRequest feeds back decoded text when finished

MessageRequest - Basic object for holding key,jobid and message

VigenereBreaker - Interface needed to implement the RMI stuff uses important rmi.Remote packages etc

WorkerThread - Does all the heavy decrypting delegation in a thread

-----------------------------
In Service there are 5 classes
-----------------------------

KeyEnumerator - Creates the quadgrams from file or passed file, scores keys, cracks cypher, returns decrypted text

Quadgram - Basic class that reads a file in then Builds,Stores and gives access to the quadgram map

VigenerBreakerImpl - Main class, Runner class, bind service etc

Vigener - This class is taken from JH's original and with only minor changes to the doEncrypt method

VigenerBreaker - Interface needed to implement the RMI stuff uses important rmi.Remote packages et

4. GitHub

https://github.com/AndyDev2013/java_distributedSystems
