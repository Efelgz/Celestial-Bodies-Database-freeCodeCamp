# Celestial Bodies Database

## Overview
This repository contains the "universe.sql" file, which is a PostgreSQL relational database built as a certification project for the FreeCodeCamp Relational Database Certification. The project demonstrates a foundational understanding of database design, table creation, and data relationships by modeling various celestial bodies.

## Database Structure
The database is structured to represent the hierarchical nature of celestial bodies in space. It includes the following primary tables:

* **galaxy:** Stores data about different galaxies.
* **star:** Contains information about stars, utilizing a foreign key to link each star to its parent galaxy.
* **planet:** Holds details about planets, linked to their respective stars via a foreign key.
* **moon:** Contains data regarding natural satellites, linked to their respective planets.

## Key Features & Constraints
* **Relational Design:** Implements one-to-many relationships across all tables using standard Primary Key and Foreign Key constraints.
* **Data Integrity:** Utilizes `NOT NULL` constraints and `UNIQUE` constraints to prevent duplicate or missing critical data.
* **Appropriate Data Types:** Makes use of various PostgreSQL data types including `SERIAL`, `VARCHAR`, `INT`, `NUMERIC`, and `BOOLEAN` to optimize data storage.

## Technologies Used
* PostgreSQL
* Bash / Linux Terminal
* SQL

## How to Run Locally
To reconstruct the database on your local machine, you need to have PostgreSQL installed. You can rebuild the database by running the following command in your terminal:

```bash
psql -U postgres < universe.sql

Author
Efe Ilgaz Köksal
