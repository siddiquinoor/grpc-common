# gRPC Hello World Tutorial

## TODO: move this to the tutorial sub-folder

A great way to get introduced to gRPC is to work through this tutorial, which
walks you through the construction of a simple client and server and introduces
various features of gRPC.

When you finish the tutorial, you will be able to

- Create a protobuf schema that defines a simple RPC service.
- Create a Java server that implements the schema interface.
- Create a Java client that accesses the server.
- Create a Go client that accesses the Java server.
- Update the service with advanced features like RPC streaming.

# Get Started

The rest of this page explains how you can set up your local machine for development.
If you just want to read the tutorial, you can go straight to the next step: [Step - 0](Step_0.md)

# Working with the code

You can follow along with this tutorial and hack on the code in the comfort of
your own computer. This way you can get hands-on practice of really writing
gRPC code.

The tutorial relies on the use of the Git versioning system for source code
management. You don't need to know anything about Git to follow the tutorial
other than how to install and run a few git commands.

# Install Git

You can download and install Git from http://git-scm.com/download. Once
installed you should have access to the git command line tool. The main
commands that you will need to use are:

- git clone ... : clone a remote repository onto your local machine
- git checkout ... : check out a particular branch or a tagged version of the code to hack on

# Download grpc-helloworld

Clone the grpc-helloword repository located at GitHub by running the following command:

```
git clone https://github.com/google/grpc-helloworld.git
```

Change your current directory to grpc-helloworld

```
cd grpc-helloworld
```

# Install Java 8

Java gRPC is designed to work with both Java 7 and Java 8.  For simplicity,
the example assumes that Java 8 is installed.  See
[Install Java 8](http://docs.oracle.com/javase/8/docs/technotes/guides/install/install_overview.html)
for instructions.

# Install Maven

To simplify building and the managing of gRPC's dependencies, the Java client
are server are structured as a standard [Maven](http://maven.apache.org/guides/getting-started/)
project. See [Install Maven](http://maven.apache.org/users/index.html) for instructions.


# Install Go 1.4

Go gRPC requires Go 1.4, the latest version of Go.  See
[Install Go](https://golang.org/doc/install) for instructions.

# (optional) Install protoc

gRPC uses the latest version of the protocol buffer compiler, protoc.

For following this tutorial, the protoc is not strictly necessary, as all the
generated code is checked into the Git repository. If you want to experiment
with generating the code yourself, download and install protoc from its
[Git repo](https://github.com/google/protobuf)