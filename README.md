# Edalex Developer Challenge

## Overview

The challenge is develop a *very* simple message board web app. It will consist of two parts:

* A [React](https://reactjs.org/) front-end written in [Typescript](https://www.typescriptlang.org/)
* A [Spring Boot](https://spring.io/projects/spring-boot) REST API back-end written in Java

Stubs have been provided for both of these (see 'Quick start'), the challenge is to build them
out to meet the below requirements. (Before starting, make sure you can successfully start the
server and client as detailed in the 'Quick start'.)

If you require additional assistance on Spring Boot, React or Typescript there are some helpful
links at the end of this README.

## Quick start

First, it is assumed you have the following items installed:

* JDK 8
* NodeJS / NPM

### Server

Go into the `server` folder and use the Gradle wrapper to make sure all is working. On Linux and
MacOS that will look like:

    ./gradlew bootRun

On Windows:

    gradlew.bat bootRun

You should see it download dependencies, build the source, and then complete a server start-up. At
which point you should be able to confirm all is working by going to
<http://localhost:8080/api/message>. That will return you a JSON response with three messages.

### Client

First, Go into the `client` folder and install the Node dependencies:

    npm install

Then start the local dev server/build environment:

    npm run start

After a few moments, you should be able to visit the client in your browser at:
<http://localhost:3000/>.

## Requirements

Your completed challenge must meet these requirements:

* Display a list of messages ordered with the most recent at the top
* Allow a user to add a message
* Allow a user to remove a message
* View a single message (i.e. a permalink)

### User Interface

It is acceptable to deliver a bare bones, plain HTML UI. However, you're invited to deliver one which
is done with [Material-UI](https://material-ui.com/).

### Data Persistence

It is acceptable to deliver with the system simply using a file (CSV, YAML, JSON, your own) for
persisting the data (no expectation of ACID compliance). However, if you'd like to demonstrate your
ability to use an ORM, you're welcome to use a file based H2 set-up.

If you do go down this path, either make sure that the configuration is embedded, or that you
provide additional documentation.

### Security

We are not expecting any security to be implemented.

## What we're looking for

A simple idiomatic React/Typescript app - not expecting Redux (you've gone too far). Backed by a
simple Java REST service demonstrating understanding of separation of concerns through application
layers.

Using Material-UI and/or an ORM are only for bonus points.

## Submission

We expect to receive back the resultant source tree - without intermediate files (most of which are
excluded by `.gitignore`). We will then build the two parts and run them to ensure
requirements compliance. (Make sure any additional instructions are included.) Then we'll undertake
a code review.

## Some helpful resources

* [Spring Boot - Getting Started: Building a RESTful Web Service](https://spring.io/guides/gs/rest-service/)
* [The “Spring Web MVC
  Framework”](https://docs.spring.io/spring-boot/docs/2.1.1.RELEASE/reference/html/boot-features-developing-web-applications.html#boot-features-spring-mvc)
* [Typescript in 5 minutes](https://www.typescriptlang.org/docs/handbook/typescript-in-5-minutes.html)
* [React tutorial](https://reactjs.org/tutorial/tutorial.html)
