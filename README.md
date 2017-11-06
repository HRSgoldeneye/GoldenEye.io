# Table of Contents

* [About GoldenEye](#about-goldeneye)
* [Inspiration](#inspiration)
* [Features](#features)
* [How will it look](#how-will-it-look)
* [Installation](#installation)
* [Application design](#application-design)
  * [Directory structure](#directory-structure)
  * [Import conventions](#import-conventions)
  * [Naming conventions](#naming-conventions)
  * [Data model](#data-model)
  * [CSS](#css)
  * [Routing](#routing)
  * [Authentication](#authentication)
  * [Authorization](#authorization)
  * [Configuration](#configuration)
* [About Us](#about-us)
* [Development History](#development-history)
    * [Milestone 1: Data and ElasticSearch](#milestone-1-data-and-elasticsearch)
    * [Milestone 2: Front End and Other Improvements](#milestone-2-front-end-and-other-improvements)
    * [DigitalOcean and Laravel Forge Deployment](#digitalocean-and-laravel-forge-deployment)

## About GoldenEye

As part of ICS-491, our group participated in the 2017 Hawaii Annual Coding Challenge and took on the challenge of making the Hawaii Revised Stautes easily accessible. Goldeneye comes from the James Bond movie of the same name. But rather on being a Soviet super weapon, it's an app made to simplify the process of accessing and updating Hawaii's laws.

## Inspiration

Besides a great challenge, the current problems with accessing the statutes is that it's very tedious looking through the statutes. With over 20,000 sections, there is no database and no way to search for a particular statute or section. There's also no way to cross reference another statute if it's listed in another staute. 

On the official Hawai’i Government Website, https://portal.ehawaii.gov/government/hawaii-legislature/hawaii-revised-statutes/, the statutes are on a file server. This means that it's another obstacle to update or edit statutes. Currently, the statutes are officially updated once a year. With this slow process, there is no consistency and typos are common for some statutes.

## Features

With our team, we plan to use the laravel framework as our foundation to creating a dynamic web application that can be accessed on ac computer or a smart phone. With mysql as our database and using the ElasticSearch package, we want to make common sense search engine that will query results a user expects to see. To increase the long term support of the app, we want to create an easy to use administrative side that allows a layman to maintain the statutes within our app. Along with the other teams creating similar solutions, we collaborated on making a free and open source scrapper that allows other developers to have all the statutes or some parts of it in a simple JSON file.


# How will it look

PC View

![image](/images/pagemain.jpg)

![image](/images/pageabout.jpg)

Mobile View

![image](/images/picture1.png)

![image](/images/picture2.png)


# Installation

For a visual guide on installing laravel and developing: use [laracasts](https://laracasts.com/series/laravel-from-scratch-2017).
First, download the PHP depenedency manager [composer](https://getcomposer.org/).

# Application Design

## Directory Structure

## Import Conventions

## Naming Conventions

## Data Model

## CSS

## Routing

## Authentication

## Authorization

## Configuration


# About Us
Team GoldenEye is one of the participants in [Hawaii Annual Code Challenge](http://hacc.hawaii.gov/) and 
the team is formed with two people. 

* [Mark Cummins](https://github.com/markrcummins)
* [Yohan Yang](https://github.com/yohanyang)

# Development History

The development process for GoldenEye conforms to [Issue Driven Project Management](http://courses.ics.hawaii.edu/ics314s17/modules/project-management/) practices. In a nutshell, development consists of a sequence of Milestones. Milestones consist of issues corresponding to tasks. GitHub projects are used to manage the processing of tasks during a milestone. 

The following sections document the development history of the UHM ICS BookMarket.

## Milestone 1: Data and ElasticSearch

This milestone started on October 2, 2017 and ended on November 6, 2017.

The goal of Milestone 1 was to implement the backend and data portion of our app. The first part was collaborating with other groups to create an free and open source [HRS scrapper](https://github.com/OpenHRS/openhrs-scraper-app). The second part was creating a relational database that could insert the JSON file that the scrapper generated. The third part was configuring the ElasticSearch package so that statutes and sections could be searched and relevant results would show. The final part was successfully deploying a live version of the app. 

## Milestone 2: Front End and Other Improvements

This milestone started on November 6, 2017 and ends on December 1st, 2017. This milestone consists of greatly overhauling every aspect of the app. This includes the front end and the back end of app. The first is utilizing the elasticsearch engine on the production version of the app and optimizing the search mapping. The second part is utilizing the CSS framework [materializecss](http://materializecss.com/table.html) and the front end framework [vue.js](https://vuejs.org/). The third part is to implement an administrative account that allows one user/account to make changes to the production version of the application. Finally, we want to implement sound software engineering principles like testing on both the desktop and mobile version of GoldenEye. 

## DigitalOcean and Laravel Forge Deployment

To test certain features and to meet the requirements of the class, our app is deployed [here](http://165.227.195.48/). Our deployment is made by creating our server on DigitalOcean and managing it with Laravel Forge. 
