
Original App Design Project - README Template
===

#GrindTime

## Table of Contents
1. [Overview](#Overview)
1. [Product Spec](#Product-Spec)
1. [Wireframes](#Wireframes)
2.  [Schema](#Schema)

## Overview
### Description
  This app will be a sports app, called GrindTime, that shows all sports specific parks that are in certain areas. Once you find the one you want to go to you can then find other people who are going to that same park and have a chance contacting them through the app to see if other athletes would like to train with you and at what time and on what day as well. This could be helpful for people who especially don't have coaches or need to find a place that fits their needs for whatever sport they need to train for. 

### App Evaluation
[Evaluation of your app across the following attributes]
- **Category: Sports

- **Mobile: This app will be mostly of that for mobile users 

- **Story: Athletes will be able to find parks to train at when they need to. For their specific sports that they are in or interested in.

- **Market: Not every athlete or person knows the best parks to go to inorder to train or practice their sports with others like themselves. This app will help with finding those specific parks and finding others as well that they could train with when needed. As well as  befriends others so they can meet up once again.

- **Habit: This sports app will be used whenever a user needs to find their park, contact other users to train with, or to just get caught up on new information pertaining to the parks and comments that others post on the parks.

- **Scope: The app will be easy to access because due to the mobility and direct information that is provided within the app such as how to utilize the app and the specifics on the different times, locations, and sports that are played in that area.



## Product Spec

### 1. User Stories (Required and Optional)

**Required Must-have Stories**

- [x] User being able to log in

- [x] User being able to sign up for an account

- [] Users will be able to make a profile

- [] User will be able to chat with other users

- [] Users will be able to scroll through out which parks are for which sport 

- [] Users will be able to comment

- [] User can log out



**Optional Nice-to-have Stories**

- [] Users will be able to post pictures 

- [] User will be able to stay logged in 

- [] user able to add a profile pic
 


### 2. Screen Archetypes

Login - Users will be able to login if they have made an account

Register- The user will need to register for an account in order to even use the app if they want to find sport parks.

Profile -  The user will be able to make a small profile for themselves so others can see if they want.

Chat Screen - This is where users will be able to chat with another or make request in wanting to train together. 

Stream screen (Home screen) - Where the main user will be able to see the parks and comments from other users.

Post Screen - WHere the user will be able to post what they are going to be doing or their comments.

Launch Screen - Shows the app launch image when loading.



### 3. Navigation

**Tab Navigation** (Tab to Screen)

Home screen

Post a comment 

Menu tab on the side:

Profile 

Locate 

Message

Post

Login 

Logout 


**Flow Navigation** (Screen to Screen)

Launch Screen => Login

Login => Homescreen

Register => Home screen

Home screen => Chat Screen

Home screen => Post Screen



## Wireframes
[Add picture of your hand sketched wireframes in this section]
<img src="https://github.com/Jodimedina9/Sport_Parks/blob/main/IOS%20App.jpg" width=600>

### [BONUS] Digital Wireframes & Mockups

### [BONUS] Interactive Prototype


### Models
![Login model](https://user-images.githubusercontent.com/32984556/111934449-6be41c00-8a8f-11eb-8f6f-d479ce532819.JPG)
![User Profile Model](https://user-images.githubusercontent.com/32984556/111934645-d2693a00-8a8f-11eb-8759-a2ea688ad027.JPG)
![Post Model](https://user-images.githubusercontent.com/32984556/111935106-be720800-8a90-11eb-8621-67825ebc6990.JPG)
![Messages Model](https://user-images.githubusercontent.com/32984556/111935234-0abd4800-8a91-11eb-8e6e-71100fade4e2.JPG)


### Networking

 Home Feed Screen
 
(Read/GET) Query all posts where user is author

let query = PFQuery(username:"Post")

query.whereKey("author", equalTo: currentUser)

query.order(byDescending: "createdAt")

query.findObjectsInBackground { (posts: [PFObject]?, error: Error?) in

if let error = error { 

print(error.localizedDescription)

} else if let posts = posts {

print("Successfully retrieved \(posts.count) posts.")

// TODO: Do something with posts...

}

}

(Create/POST) Create a new like on a post

(Delete) Delete existing like

(Create/POST) Create a new comment on a post

(Delete) Delete existing comment

(Read/Post) search and post location 

Create Post Screen

(Create/POST) Create a new post object

Profile Screen

(Read/GET) Query logged in user object

(Update/PUT) Update user profile image

Message screen

- (Create/ Send) Create new message

-  (Read/Get) Read and Reply to messages

- Login Screen

- (Insert) Insert username 

-  (Insert) Insert password 



Register Screen (New Account) 
- (Create/Get) Insert First Name

- (Create/Get) Insert Last name

- (Create) Create new username 

- (Create) Create new Password


Gif: 


Here's a walkthrough of implemented user stories:

<img src=' https://imgflip.com/gif/53k2ua ' width='' alt='Video Walkthrough' />

