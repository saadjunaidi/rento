# Rento - Home Away from Home

- Make sure you have PostGREs installed with a DB created with a username and password (say user/password).
- Make sure you have JDK 1.8 with javac added to PATH.

javac -version
javac 1.8.0_60
java -version
java version "1.8.0_60"
Java(TM) SE Runtime Environment (build 1.8.0_60-b27)
Java HotSpot(TM) 64-Bit Server VM (build 25.60-b23, mixed mode)

Both the versions should me same (and >= Java 1.8)

$ git clone git@github.com:saadjunaidi/rento.git
$ cd rento
$ cd conf
$ vim application.conf      (Edit as required)
$ ./activator run

or on Windows

cmd\> cd <project folder>
cmd\> activator run

This would download all the dependencies, build, and run the project on default port 9000.
Next open your web browser and point to: http://localhost:9000/


Install and configure IntelliJ IDEA

**> Install IntelliJ IDEA and then configure it for Scala Plugins.
	1. Go to Configure -> plugins (or from some where else).
	2. search and install scala plugin (this will install all sbt, and play related stuff)

**> Import the project from existing source and then add the latest JDK location.
	1. Import Project from existing sources.
	2. Now import from external model and select "SBT" from Import Project dialog.
	3. Now Select project SDK from dropdown if available.
			OR
	3. Create New SDK from the path of the latest java version.

EDIT: saad (Thur June 9 18:16:26 IST 2016) Or just File > Open (And locate the path of your checkout)

**> Refresh SBT somehow (you need to figure it out, you are the dev, are not you)

Done.
