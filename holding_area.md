# Holding Area


> Reserved for heavy topics, controversial subjects or content that needs immediate resolve and decision. Make no mistake, this book is for teens and has angles in it that make the reader aware we are serious about the direction of our Global community. The holding area is ultimately for organizing important content before inserting it into the main text.

### ON PROBLEM SOLVING

### ON PRIORITIZING

### ON CONCENTRATION

### ON THE TAO

### INCLUSION

### ON BEST PRACTICES

### ON OFFICE CULTURE

### ON WORK ETHIC

### ON BALANCE

### ON WELL ROUNDEDNESS

### ON RACISM

Racist. I am a racist. I believe that all races should have the right to protect their race against wrongdoing. I do not hate other races, I respect them. What I do hate are people that do shitty things, unfair things, unjust things. I hate governments that lie and cheat for profit. I hate educators that fail to do their job, and parents the same. I hate inequality. I believe that all sides of town deserve equal opportunity. 

Today @sama put up this image. A Racist image of our countries SAT scores. 
![](http://res.cloudinary.com/dzryfxssm/image/upload/v1475935813/racist_coeqr6.jpg)

But if you notice, we are also all doing bad, together. Except for Asians apparently - props Asia! 

When we created this book, we interviewed counselors and said, what's up with this? They said, particularly when race concentrations are high, in certain areas, or with certain patterns in the home, the kids have no motivation. They are not inspired. 

Before we even met these people this came to our attention, I launched our first campaign stating:

"This book will inspire you kids to want to learn about electrical engineering and computer science."

That's all I knew. As a white (Italian, Polish, Native American) man, trying to teach his own kids his skill, this is what I did. My entire company was formed on the idea that I needed to teach my young. Train my sons in Soccer and Tech, and culture my daughter in math and arts. This is what I've spent the past 10 years on, and will continue to do until I am no longer able. 

The dialogue has to change people. It must go from black, white, yellow, green to => win, learn, share, use wisely. Each race has the right to focus on their own success, but not at the expense of hurting another race, as generating negativity will only hold your race back. 

The answer isn't necessarily that we all come together. Each of our races need to do a better job inspiring our kids to be smarter, to live better and to stay away from trouble. All too often, we as parents incite violence, encourage bad behavior and fail to watch after our own young. I wrote this book as a personal contribution towards the part of our society that I know believes in this, and to persuade the others to cut the shit. 

No excuses, there are plenty of tools to help, plenty of example methods for raising your young.  Stop, make the time, lead by example and develop a style for how you teach.



### HOW CODERS INTERACT ON NEW PROJECTS


> Clean this up Franchino and get out of sight.


franchino [10:09 AM]  
Hey

[10:09]  
want to talk about another project?

[10:09]  
I think you’ll like this one

[10:10]  
might be an ionic angular 2 or react native project

[10:10]  
everything you’ll be doing is very compact

[10:10]  
ie. first task

[10:10]  
1. Create a function that scans a QR code and redirects user to a route.

[10:11]  
2. Hit this “CURL METHOD” and parse JSON to make display like so on a page.

[10:11]  
3. Create an Auth0 membership process with a social login.

[10:11]  
yes or no

mylesgearon [10:12 AM]  
Sure!

[10:12]  
I'll be doing a lot of learning on that one though, I haven't dipped my toes into mobile

franchino [10:12 AM]  
I’m really good

[10:12]  
stick with me

[10:12]  
you’ll be fine

[10:12]  
I’ve worked on at least 20 Ionic apps

[10:13]  
there’s a lot of stuff already out there...

[10:13]  
but we will also get a chance to learn it deeply

[10:13]  
the way I’m going to judge which platform to use right now is based on several factors

[10:14]  
1) When all the major tasks are looked at, which framework has better tested implementations and resources, more active git projects, etc.

[10:14]  
2) Which app will give me PWA

[10:14]  
sorry, rather which framework will give me greater chances at PWA or multi-tennat

[10:15]  
I am HUGE on hypermedia

[10:15]  
and APIS as  a state machine

[10:15]  
and REDUX only adds to my ideas

[10:15]  
especially when dealing with Gamification,

[10:15]  
it’s almost to me as if Redux were designed for more intelligent aplications

mylesgearon [10:16 AM]  
Yeah, Redux is a lifesaver for anything complicated.

[10:16]  
You're talking about deciding between ionic and react native

[10:18]  
That sounds like a lot of fun either way! Let me know what you decide and I'll start learning

franchino [10:19 AM]  
weigh in here newb

mylesgearon [10:21 AM]  
Oh, well I don't know much about either, but I do know quite a bit about react, and I'm imagining native isn't much of a leap from there. But let me look at them for a bit

franchino [10:21 AM]  
so there here’s what you need to know about me…

[10:21]  
I’m a PWA guy

[10:22]  
Progressive Web App believer

[10:22]  
I believe in Redux as a better paradigm for highly stateful, multi-tennat apps,

[10:23]  
but I also believe that APIS can be excellent managers of State

[10:23]  
hence Hypermedia APIS

[10:23]  
I’ve been a designer of both systems a very long time

[10:23]  
I have github projects with a lot of use dating back 5 years already pushing PWAS

[10:23]  
and most of my best software work invovled hypermedia thinking

[10:24]  
ie. a lot of key value pair stuff, redis, hashes, etc.

[10:24]  
dictionaries

[10:24]  
I’m also a big fan of great UI libraries, on the front-end

[10:24]  
stuff like Material UI

[10:24]  
and React has a really nice implementation of that

[10:25]  
as a complete PWA ready platform

[10:25]  
React Native is not there

[10:25]  
it’s kinda sperate from React

[10:25]  
it further divides the idea

[10:25]  
that you should write once, run everywhere

[10:25]  
I don’t like the idea of maintaining a Swift app, Android app, web app and mobile web app all seperately

mylesgearon [10:26 AM]  
Yeah, my understanding is that with native you don't get to transfer much more than the logic

[10:26]  
?

franchino [10:26 AM]  
I believe that you should write one JS set of controllers, modules, components or whatever...

[10:26]  
angular 2 is a lot more like react from this perspective

[10:27]  
import { Component } from '@angular/core';
@Component({
 selector: 'my-app',
 template: '<h1>My First Angular App</h1>'
})
export class AppComponent { }

[10:27]  
import { NgModule }      from '@angular/core';
import { BrowserModule } from '@angular/platform-browser';
import { AppComponent }   from './app.component';
@NgModule({
 imports:      [ BrowserModule ],
 declarations: [ AppComponent ],
 bootstrap:    [ AppComponent ]
})
export class AppModule { }

[10:28]  
I think NG Cordova has the most amount of coverage in terms of an API that wraps all native IOS and Android native functions

[10:28]  
http://ngcordova.com/
 ngcordova.com
ngCordova - Cordova Plugins with AngularJS Magic
ngCordova - Simple and powerful AngularJS Services for Cordova and Phonegap (10KB)


[10:28]  
this is where it get’s dicy with native

mylesgearon [10:45 AM]  
It seems that's been replaced with http://ionicframework.com/docs/v2/native/
 ionicframework.com
Ionic Native: Harness the power of Native APIs
Ionic makes it incredibly easy to build beautiful and interactive mobile apps using HTML5 and AngularJS. 
 
 

[10:45]  
for ES6/TypeScript and Angular 2

franchino [10:49 AM]  
Right

[10:49]  
yeah, I suspected that

[10:49]  
cordova was married to phone gap

[10:50]  
and Ionic was sorta cheating with them around 1.0

[10:50]  
fuck I should have known that I was wondering when I did a search for cordova just now

[10:50]  
http://ionicframework.com/docs/v2/native/

[10:50]  
good

[10:50]  
proud of these guys

[10:50]  
i know the founder

[10:50]  
Max Lynch

[10:51]  
He got funding from Lightbank

[10:51]  
he was in the cohort after me

[10:52]  
This came recommended by Mike Harrington

[10:52]  
https://github.com/rangle/angular2-redux-example
 GitHub
rangle/angular2-redux-example
angular2-redux-example - Angular 2 Redux Starter Repo 
 
 

[10:52]  
so I guess, proof of concept would be….

[10:53]  
angular2-redux based starter app with a QR code reader that can open up a route.

[10:54]  
and if it’s PWA, the same exact codebase should be able to generate and distinguish between a native app, a mobile web app and a web app (realizing that you wouldn’t have a QR coder on a web app, rather another method).

[10:58]  
there’s also this

[10:58]  
https://github.com/ngrx/store
 GitHub
ngrx/store
store - RxJS powered state management for Angular2 apps, inspired by Redux 
 
 

franchino [11:19 AM]  
Maybe we start here?

[11:19]  
https://github.com/ngrx/example-app
 GitHub
ngrx/example-app
example-app - Example app showcasing the ngrx platform 
 
 

mylesgearon [11:20 AM]  
Okay, I'll work on that. I'm going to try to get set up w/ ngrx and ionic 2. It'll be a second there

franchino [11:20 AM]  
I’m going to give you something to pull

[11:20]  
hang tight

[11:20]  
wow

mylesgearon [11:20 AM]  
I'm going to start with a tutorial I found if you don't mind, I have A LOT of learning to do in this stack

franchino [11:20 AM]  
yup

[11:21]  
the app I just sent you is an NGRX starter

[11:21]  
you can do a tutorial if you want

[11:21]  
let me know which one you’re doing and how it goes!

mylesgearon [11:21 AM]  
Yeah, I found one that's on ngrx in ionic 2

franchino [11:21 AM]  
there might be a good thinkster.io crash course on angular 2

mylesgearon [11:21 AM]  
http://gonehybrid.com/a-beginners-guide-to-using-ngrx-in-an-ionic-2-app-part-1/
 Gone Hybrid | Learn to develop Hybrid Mobile Apps with Angular and Ionic
A Beginner's Guide To Using ngrx In An Ionic 2 App - Part 1
In this tutorial, we'll have a look at what ngrx is and how it can help you manage application state in your Ionic 2 app, or any other Angular 2 app for that matter. This tutorial is part of a multi-part series: Part 1 - Setting up Store, Actions and
Written by
----------------
Ashteya Biharisingh

Filed under
----------------
Ionic 2, Angular 2, TypeScript, ngrx, RxJS

July 4th at 1:04 PM

franchino [11:21 AM]  
Nice!

[11:21]  
i’ll go though this as well

[11:21]  
this is exciting bruh!

mylesgearon [11:22 AM]  
I'm very exciterrirified (edited)

franchino [11:22 AM]  
you’ll do fine

[11:22]  
take 6 commits a day

[11:22]  
to keep the doctor away

franchino [3:50 PM]  
bruh

[3:50]  
what’s up

mylesgearon [3:51 PM]  
I'm just reading about different parts of the stack, something needs doing?

franchino [3:51 PM]  
what’s your github

[3:51]  
git

[3:51]  
username

mylesgearon [3:51 PM]  
mityadsch

franchino [3:51 PM]  
no

[3:51]  
all good

[3:52]  
https://github.com/frangucc/g3/invitations


