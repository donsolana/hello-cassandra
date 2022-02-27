# hello-cassandra

## Introduction

This project demonstrates the data modelling process for Apache Cassandra, a noSQL database. The database is here is for a music streaming website. Nosql databases are optimized for fast writes. To design for faster reads tables have to be entirely denormalized with queries in mind. In other words, each table in the Cassandra data base is modelling based on it's unique query outcome, with data redundancy(overlaps between tables) permitted. in some sense this is an easier process that with relational databases. The trick however lies majorly in how data is partioned and sorted across nodes.

## How to run project:

Project is a jupiter notebook. That follows these steps:

1. We walk through file folder with data.
2. Read in CSVs with all contain individual events
3. We extract relevant columns(values) from each CSV and read them into new CSV that will house all events
4. We then initiate the Cassandra cluster and define a key space.
5. We create all our tables within this keyspace.
6. We validate our table by running the queries they where designed for.
7. Drop tables and close connections

## Tools
1. Python Cassandra driver aptly named "cassandra"
2. Pandas for data manipulation
3. OS and glob for crawling through file repository

## To-do:
1. Modularize code

