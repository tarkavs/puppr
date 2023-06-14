# PuppR ~ *Anything is pawssible*

![logo](https://i.imgur.com/zg49V5K.png)

# Introduction

## The Project
As a dog owner, I have experienced the struggle of moving to a new place and not knowing anyone else with a dog. Dogs need to socialize too! That's why I created **PuppR**.

[**PuppR**](https://puppr.best/) is a dating site for dogs! Dog owners can create a profile for their pup and start swiping through other dogs in their area. If they want to meet a dog, they can "like" their profile, and if that dog likes them back, it's a match! From there, the two users can decide to contact each other and organize a playdate for their dogs. If they don't like a dog, they can simply "pass" on it.

Other features include editing the dog's profile, modifying user settings, and a "previous" button to revisit the previous profile.

## The Context
This project was a personal endeavor that I undertook. I wanted to create a fun and useful platform for dog owners to connect and set up playdates for their furry friends.

## Blog Post
To learn more about my journey of creating **PuppR**, you can check out my blog post on Medium: [PuppR: Bringing Dogs Together](https://link.medium.com/iM1VuBXZAAb)

# Architecture

## Overview
**PuppR** is a web application built mainly with JavaScript. The front-end is developed using Vue.js, a popular JavaScript framework. The application communicates with a Firebase backend, which provides features such as authentication and database storage.

![architecture](https://i.imgur.com/fSbo6ho.jpg)

## Vue.js
I chose to use Vue.js as the front-end framework for **PuppR**. Vue.js is known for its simplicity and ease of use, making it a great choice for a project like this.

The different sections of the app are implemented as Vue components. Each component represents a specific page or feature of the application. The main component, "App," serves as the entry point of the app.

The components are connected using Vue Router, which handles the routing and navigation between different components. The routes are appended to the application's URL to provide a seamless user experience.

The state management in the app is handled by a Vue.js store, which is defined in the `store.js` file. The store allows data to be shared and accessed across components without the need for prop drilling or event buses.

## Firebase
For the backend and database functionality, I chose Firebase. Firebase provides a range of tools and services that greatly simplify the development process.

### Firestore
Firestore, a NoSQL document database, is used to store the majority of the application's data. User information, such as display names, dog profiles, likes, and matches, are stored in Firestore. Firestore's quick database calls ensure a responsive and seamless user experience.

### Authentication
Firebase Authentication is used for user authentication. It handles the signup and login process, ensuring that only authenticated users can access the app's features.

### Cloud Firestore
Cloud Firestore, a cloud-hosted NoSQL database, is utilized to store users' dog photos. The images are uploaded to Cloud Storage, and the corresponding URLs are stored in Cloud Firestore. This allows for easy retrieval and display of dog photos within the app.

# Acknowledgments

* Tarkav Sunday - For the dedication and effort in developing **PuppR**.

* Inspirational Dog Owners - For inspiring the creation of **PuppR** and providing valuable insights into the needs of dog owners.

* Vue.js Community - For the continuous support and development 
