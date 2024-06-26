"VERY SIMPLE SHIP GAME"

A fun personal project, my first venture into 2D game programming using 
the Java libGDX framework.  The sprites are all homemade in GIMP on Gentoo Linux.  
The laser sounds are homemade using Audacity to alter recordings of my electric 
guitar hitting a note.

-------------------
GENERAL NOTES:
-------------------

The project has Desktop, Android, HTML and iOS modules that are automatically managed while only the class files in the "core" directory are usually edited and added to.  Still working on iOS and Android implementations.

It's currently setup with Gradle.  Download the latest version of Android Studio IDE and import the project if you want to work with the code.  

If you just want to run it on your desktop without opening a coding environment, you can simply run " ./gradlew desktop:run  ".

You can build a jar to run on Linux, MacOS or Windows with ./gradlew desktop:dist.  The jar will appear in /ProjectRoot/desktop/build/libs as " desktop-1.0.jar ".

To build an executable for your OS, run the corresponding " pack-${OS}.sh " bash script.  If you are on Windows, you can access bash through git-bash, available here: https://git-scm.com/downloads

-------------------
 HTML VERSION:
-------------------

To test the html version, you can spin up an http server.  Running this from your IDE terminal will do fine on a Linux system:

python -m http.server 8000
 
 Then go to  http://localhost:8000 and navigate to html/build/dist in that browser window.
 
 You can start the server also with " ./gradlew html:superdev ", then connect to http://localhost:8080/index.html (current config) or http://localhost:8080/html/ (older Gradle configuration with Jetty plugin).
 
 Helpful links:
 
 https://libgdx.com/wiki/deployment/deploying-your-application
 
 If you are trying to run a jar of it on Macintosh computers, you need to add the -XstartOnFirstThread option, giving java -jar --XstartOnFirstThread desktop-1.0.jar
 
 
