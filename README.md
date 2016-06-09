# Rento - Home Away from Home

- Make sure you have PostGREs installed with a DB created with a username and password (say user/password).
- Make sure you have JDK 1.8 with javac added to PATH.

javac -version<br />
javac 1.8.0_60<br />
java -version<br />
java version "1.8.0_60"<br />
Java(TM) SE Runtime Environment (build 1.8.0_60-b27)<br />
Java HotSpot(TM) 64-Bit Server VM (build 25.60-b23, mixed mode)<br />

Both the versions should me same (and >= Java 1.8)

$ git clone git@github.com:saadjunaidi/rento.git<br />
$ cd rento<br />
$ cd conf<br />
$ vim application.conf      (Edit as required)<br />
$ ./activator run<br />

or on Windows<br />

cmd\> cd <project folder><br />
cmd\> activator run<br />

This would download all the dependencies, build, and run the project on default port 9000.<br />
Next open your web browser and point to: http://localhost:9000/


Install and configure IntelliJ IDEA<br />

** Install IntelliJ IDEA and then configure it for Scala Plugins.<br />
	1. Go to Configure -> plugins (or from some where else).<br />
	2. search and install scala plugin (this will install all sbt, and play related stuff)<br />

** Import the project from existing source and then add the latest JDK location.<br />
	1. Import Project from existing sources.<br />
	2. Now import from external model and select "SBT" from Import Project dialog.<br />
	3. Now Select project SDK from dropdown if available.<br />
			OR
	3. Create New SDK from the path of the latest java version.<br />

EDIT: saad (Thur June 9 18:16:26 IST 2016) Or just File > Open (And locate the path of your checkout)<br />

** Refresh SBT somehow (you need to figure it out, you are the dev, are not you)<br />

Done.
