# Smart-schedule-for-smart-grid
Implemented a integrated framework consisting of software for two servers a home server for each particular home and a utility server for a community
The servers codes were written in hadoop (JAVA) with multiple map-reduces to deliver the result for more than a million home data
The most optimized schedule was determined using simulated annealing algorithm running in the servers with the user provide details through mobile application
Server client interface was achieved using HTTP POST and GET methods, PHP scripts and JSON objects

————————————————————————————————————————————————————————————————————
				README
————————————————————————————————————————————————————————————————————

1: The server codes and the utility codes have been provided separately.
2: for home server:
	1.	open eclipse
	2.	create a java project named FinalProject and create a package named grid
	3.	copy paste all the java code into the package
	4.	change the path for price cvs file in read file.java, (variable csvFile)
	5.	change the username and password for mysql connection in all the files.
	6.	run the collect.java that will start the home server
3: For utility server:
	1.	open eclipse
	2.	create a MapReduce project and import all libraries for running hadoop
	3.	create a package called utility and paste all the codes from the utility code folder
	4.	change the mysql username and password for mysql connection in all the files
	5.	provide the proper location for input and output files for hadoop and output in local directories.
	6.	provide the arguments for input and output for server.java
	7.	run server.java that wills start the utility server.
4: Setting up the servers.
	1.	open phpmyadmin.
	2.	import the two sql files provided, that will setup the users database and grid utility database for both home and utility
	3.	copy the htdocs folder into your server htdocs location.	
5: The mobile app:
	1.	open android studio
	2.	import the project SmartGrid.
	3.	change the IPhome and IPutil in app.java with the correct IPs of home and utility respectively
	4.	run the application in an android phone and access all the features of the project.

