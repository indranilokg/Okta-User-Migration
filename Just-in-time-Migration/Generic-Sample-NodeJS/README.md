# Sample Just-In-Time Migration - Local Store

This sample application is based on the steps defined in the [Okta Developer Guide](https://developer.okta.com/docs/guides/password-import-hook/nodejs/overview/).

It leverages a local file based user store. The user name and password combinations are stored in a local `users.json` file. The application can be easily adopted to verify aganinst a remote store instead.

## Installation
```
git clone https://github.com/indranilokg/Okta-User-Migration.git
```

## Project setup

* From the project root folder, install the dependencies.

```
$ npm install
```
* From the project root folder, change `users.json` to store your target user name and password combinations

### Deploy to Heroku

* Get a free [Heroku account](https://signup.heroku.com/), if not already there.

* Open command line and go to the project root folder. 

```
$ cd Okta-User-Migration/
```
* Login to Heroku and create an application

```
$ heroku login

$ heroku create oktpasswordhookdemo <- provide a different name
```
* Deploy the application

```
$ git subtree push --prefix Just-in-time-Migration/Generic-Sample-NodeJS heroku master
```
* After deployment, the application should be available at 

```
https://<your-app-name>.herokuapp.com
Example -
https://oktpasswordhookdemo.herokuapp.com
```

## Okta configuration


## Test the migration
