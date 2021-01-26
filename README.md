# RTUChat_RAE411_Final

My Final Project during the course RAE411 "Telecommunications Software" at Riga Technical University 

## "Riga Technical University Student Chat Online"
### Telecommunications Software Final Work

A simple online chat to be used between RTU Students with React and Firebase. 
Only 100 simultaneous connections limited due to low space on the free Trial of Firebase.

by Alexandre Greiner | 200ADM042


![App](https://user-images.githubusercontent.com/62612245/105652801-7bdde600-5eba-11eb-8f2e-32a515a027e6.JPG)


... Currently being edited 


#### Inspiration

For this project we had to create a Web Application using different features and tools that we learned from our "Telecommunication Software Technologies" Course such as :  GitHub, GitLab, Visualise data with D3js library, API Gateway, Amazon AWS, HTML/CSS, JavaScript, GraphQL,React.Js, Node.Js. 

Basically I wanted to implement a new Chat platform for RTU students to communicate with. Indeed, with the arrival of COVID19 during my time there in Riga, we had almost no lessons at university at all and mostly online courses, zoom meetings to exchange and be mixed with international and local students. Hence the lack of proximity and social life between students, my RTU Chat Room would allow students to meet, interact and discuss in other fields than just studies and zoom chat during lessons !

#### What the project does

RTUChat is an online cloud ChatRoom, with Google Accounts Authentification for each student, free to use and limited to a maximum of 100 connections at the same time (can be improved with sufficient further investment). Furthermore, people from all around the world can connect to this chat, hopefully it will be accessible and shared between students on ORTUS only to talk about big subjects, debates, or even help in homeworks. The project also has some rules of good behavior for a wholesome community without toxicity. "Bad words" can be traced and users that says this kind of mean language or spamming the chat can be banned for life from this Chat Room Server. 

Chat is only available after you signed in !

#### Project Architecture

Combining React & Firebase to build from scratch a Basic Chat App. 
Back End : FireBase
Front End : React.JS, HTML, CSS

- Firebase User Authentification with Google accounts
- RealTime Data Streams using React Hooks
- Serverless Cloud Functions from Firebase like bad words filters and anti-spam.

Each message is a document in the Firestore DB, it contains :
- Text
- UserID
- Timestamp 

I made a query to the database for the most recent messages, if I change the data in the backend the React App will update with the most recent messages on the front end 
= REAL TIME SYNC

#### Installation Instructions

First run these lines to create an initial React Project and open it in VSCode.
'''
npx create-react-app RTUChat
code RTUChat
'''
There are two extra dependencies to install (Firebase & React Firebase Hooks) :
'''
npm install firebase react-firebase-hooks
'''

Create a firebase project on their webpage : https://console.firebase.google.com/u/0/ and paste all the config in the .initializeApp section of your App.js





