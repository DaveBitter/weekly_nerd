# Google's Firebase and why you should check it out
![google firebase](assets/hero_3.jpg)

During a talk by [Q42](https://www.q42.nl/) by Guido Bouman [Firebase](https://firebase.google.com/) came up. I never heard of Firebase so I decided to see what it is and how I can make use of it.

## What does it do?
Firebase is a platform by Google to build you app on. You can build apps for the web, Android and IOS. I will take a look at building apps for the web since that is what I do. It provides many of the functionality that you will need when building a webapplication. Firebase provides, but is not limited to, the following functionalities:

* [Authentication](https://firebase.google.com/products/auth/)
* [Realtime Database](https://firebase.google.com/products/database/)
* [Crash Reporting](https://firebase.google.com/products/crash/)
* [Cloud Functions](https://firebase.google.com/products/functions/)
* [Cloud Storage](https://firebase.google.com/products/storage/)
* [Performance Monitoring](https://firebase.google.com/products/performance/)

## Cool, but I can already do this
That's what I thought. But then I started to thing about setting up an webapplication with all this functionality. Let's take authentication for instance. A package like [Passport](https://www.npmjs.com/package/passport) can handle this perfectly. [PouchDB](https://pouchdb.com/) can be used for a realtime database. So on, so on. You will have more options to customize every part of your application, but is this always needed?

Most of the time, no! I like to use a platform like Firebase to quickly build a robust application without all the hassle of setting up and syncing up all the moving parts. I often find myself being somewhat of a know it all. "Cool, but i can already do this" was actually the first thing that popped in my head.

## Why should I check Firebase out?
Get your ideas out there! If you go through the documentation and the promotional video's all they talk about is how you can use this to make a solid, robust and scalable webapplication. But his is not what I like to use it for. I like to use it as a tool to quickly get an idea out there.

A lot of developers been there. You get a cool idea and want to quickly build an webapplication out if it. Whether you use for a job interview or you just want to test a prototype. You soon realize that building the functionality isn't the hardest thing in the world, but you can not start building that part until you've done your chores. By chores I mean building the basic foundation your webapplication will rely on. I've often found myself losing that excitement and creativity because of this.

Imagine building this webapplication that shows you the nearest pub that matches with your recent check-ins on Facebook. After showing this you can like or dislike the proposed pub. It will then save this to your account. I immediately start thinking about features. How can I make this pub matching system. Should it look if friends are there? Can you rate a place afterwards for other users. All cool stuff, but before I can get started on it I need to the chores like a building a database and handling authentication. By using Firebase I can quickly set this basic foundation up and start building the cool functionalities. With the extra time I can iterate over the webapplication and test with users.

## Cool, where do I start?
The first Firebase app I build was the [chat app example](https://codelabs.developers.google.com/codelabs/firebase-web/#0) Google provides. It touches the surface on most of the functionalities that you will need. It's a great starting point to start learning implementing Firebase into you webapplication. Let's create something amazing with it!

## Resources
[Firebase Documentation](https://firebase.google.com/docs/)
