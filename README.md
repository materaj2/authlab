# Authentication Lab

Welcome to the Authentication Lab. The lab is a selection of challenges all related to authentication or authorisation. They are all taken, in some way, from real world examples I've come across during tests or have been suggested by other testers.

You can play the latest version of all the challenges in my <a href="https://authlab.digi.ninja">online version</a> or grab the code from here build your own lab. The lab is written in Golang and should be fairly easy to install and get running.

For more information, see my <a href="https://digi.ninja/projects/authlab.php">project page</a>. This also contains more information and walkthroughs for all the labs in case you get stuck.

## Installation

First you will need Go setup on your machine, I'll leave that up to you to work through as there are plenty of resources out there to help with that.

Once you have a working version, you can get the lab by running:

```
go get github.com/digininja/authlab
```

You might get a warning about the lack of Go files, don't worry about this, it is not a problem.

This will download the project into your go source directory, probably <code>~/go/src/github.com/digininja/authlab</code>. Change into that directory and run:

```
go get -d ./...
```

This will download and install all the dependencies.

The application uses the Revel framework to handle all the web stuff. At the moment, there is a bug which prevents it from working correctly the first time it is started up, to get round this, you need to run the binary as follows to set everything up correctly:

```
~/go/bin/revel version
```

Assuming this runs OK, and does not give any errors, you are good to go.

## Starting the lab

You can start the lab with the following command:

```
~/go/bin/revel run -a github.com/digininja/authlab/
```

Then browse to <http://localhost:9000>
