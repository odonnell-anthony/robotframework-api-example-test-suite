# README #

![Robot framework](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e4/Robot-framework-logo.png/250px-Robot-framework-logo.png)

Robot Framework API automation example using [Mark Winteringham`s](https://twitter.com/2bittester) -  [Restful-Booker](https://restful-booker.herokuapp.com/)

By default this is using the live online version of RestfulBooker, but RestfulBooker can be ran locally, you can grab off git hub [here](https://github.com/mwinteringham/restful-booker)

Documentation for the API can be found [here](https://restful-booker.herokuapp.com/apidoc/index.html)

### Who is this repository for? ###

Newcomers to Robot Framework interested in automated API testing, looking for examples

### What is Robot Framework? ###

Robot framework is a python based, open source test automation framework with great extensibility. Robot framework is cross platform and will run on Mac, Linux and Windows. 

See [here ](https://robotframework.org/)for Robot Framework home page


### What exactly is this? ###

A basic Robot Framework API test suite with the following tests:

* Obtaining Auth Token
* Get All Bookings IDs
* Add New Booking
* Validate New Booking Details
* Get New Booking ID By Name
* Get New Booking ID By Date
* Update New Booking
* Partial Update New Booking
* Delete All Bookings <- commented out by default

The following supporting librarys are used in this suite alongside some of the built in librarys...

[JSON Validator](https://github.com/peterservice-rnd/robotframework-jsonvalidator)

[RequestsLibrary](https://github.com/bulkan/robotframework-requests)



### How do I get set up? ###

* Install [Python 3](https://python.org/)
* Clone or download this repository
* Using the command line navigate in to the project folder and execute the command ```pip install -r requirements``` this will install robot framework, robot framework and the required supporting library's and their dependencies

Once everything has been installed you can run the test suite from the command line in the projects folder with the command```robot .\api.robot``` 

By default it will run on the live site on the web, this can be changed at the command line to point to a local instance of restfulbooker by running ```robot -v BASE_URL:127.0.0.1:3001 .\api.robot``` or changing the ${BASEURL} variable in the api.robot file


### Who do I talk to? ###

* Anthony O`Donnell - [LinkedIn](https://www.linkedin.com/in/anthonyodonnell)