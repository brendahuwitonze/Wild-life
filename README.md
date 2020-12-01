# WILDLIFE-TRACKER
## DESCRIPTION
Wildlife Tracker is an app that allows one to record sightings of various animal,It allows one to create rangers,locations,animals and sightings. It also allows you to view rangers locations sightings and animals. One can also view sightings a ranger has made and locations with the sightings that have occured in them.

### Author
[UWITONZE BRENDAH](https://github.com/brendahuwitonze)

## setup of the database
In PSQL:
* CREATE DATABASE wildlife_tracker;
\c wildlife_tracker

* CREATE TABLE animals (id serial PRIMARY KEY, name varchar,type VARCHAR,health VARCHAR,age VARCHAR);

* CREATE TABLE locations (id serial PRIMARY KEY,name VARCHAR);

* CREATE TABLE locations_sightings (id serial PRIMARY KEY,location_id INT,sighting_id INT);

* CREATE TABLE rangers (id serial PRIMARY KEY,name VARCHAR,badge_number VARCHAR,phone-number INT );
CREATE TABLE rangers_sightings (id serial PRIMARY KEY,ranger_id INT,sighting_id INT);
* CREATE TABLE sightings (id serial PRIMARY KEY,animal_id INT,ranger_id INT,location_id INT,time TIMESTAMP);
CREATE DATABASE wildlife_tracker_test WITH TEMPLATE wildlife_tracker;

#### To run the database locally
* Go to DB.class in main/java folder and make necessary changes
* Go to DatabaseRule in test/java folder and make necessary changes

### TECHNOLOGIES USED
* JAVA
* Heroku
* CSS
* HBS







