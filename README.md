# StudyMate
This is a project made by Wuhan University International Students of the year 2022 for the Requirement and Modeling class. 
The project's objective is to complete a requirement document for a system introduced by the students. 

## What is StudyMate?
StudyMate is an exceptional interactive website designed exclusively for individuals seeking to engage in group study. With StudyMate, you can easily connect with like-minded individuals by joining or creating study groups, participating or sharing resources in the
post sessions, as well as engage in the General Library of StudyMate, and even post-meeting details to ensure smooth coordination with your study partners.

## Requirement Document Draft File
https://docs.google.com/document/d/1IJ-cV1o2Ka36fiWwwgnNiymw2SvC3ndocS-qIBZWNsw/edit?usp=sharing

## Work Update
| Date | Week | Description |
| :----: | :---: | :------------------------------------: |
| 2/4/2024 | Week 6 | Domain Model, Use Case Model |
| 5/4/2024 | Week 6 | System Sequence Diagrams |
| 16/4/2024 | Week 8 | Domain Model 2.0, Use Case Model 2.0 |
| 17/4/2024 | Week 8 | Introduction, System Design (Domain Model) |
| 28/4/2024 | Week 10 | System Sequence Diagram |
| 7/5/2024 | Week 11| Package Diagram, Sequence Diagram |
| 8/6/2024 | Week 15| Class Diagram, Deployment Diagram & Activity Diagram |
| 11/6/2024| Week 16| Final version 1.0 |
| 19/6/2024| Week 17| Final version 2.0 |

##  1 Introduction
As the landscape of education evolves, students encounter new challenges in their learning journey. The increasing complexity of academic subjects, coupled with the need for collaborative learning in today's fast-paced world, has prompted the development of StudyMate. Recognizing the difficulties students face in finding suitable study groups, sharing knowledge effectively, and 
fostering a sense of community, StudyMate aims to bridge these gaps. By providing an interactive platform that facilitates group study, knowledge exchange, and community building, StudyMate 
strives to enhance the overall learning experience for students in universities and beyond.
In this document, we will see the different software modelings and how they are modeled. Furthermore, we will look at the purpose, intended audience, and scope of this document and project.

## 1.1 Document purpose
The main purpose of this document is to provide details of the UMLs and software modelings of the StudyMate web application which will focus on some main diagrams and patterns used in the modeling of it. The intention of the document is to help audiences related to the Studymate web application to understand how the system is modeled, furthermore, it is also intended to show the project consultant the strengths or weaknesses of the system before the team starts detailed designs. Finally, the project consultant and team members could able to validate whether the web application meets the expected software modeling.

## 1.2 Project scope
This document aims to provide a platform where university students and individuals are allowed to:

<br>-Explore the available study groups for joining.
<br>-Create or join study groups.
<br>-After joining groups you can participate in the group discussions.
<br>-Participate in the ranking(of study groups).

The website will serve as a productive hub for educational support, foster a community of learners, and incentivize the learning of users with its different activities.

## 1.3 Intended audience
The intended audience for this document includes:
<br>-Project developers
<br>-Project managers
<br>-Project designers
<br>-Project implementers
<br>-Project testers
<br>-Project stakeholders
<br>-Documentation writers



## Domain model
![StudyMate_Domain Model](https://github.com/MetaKt/StudyMate/assets/91473477/a0d0d9b0-3c8e-4f9e-9524-babb4306e049)

 Figure Logical Structural View: Domain Model Diagram </p>

The domain model provides an abstract, high-level overview of the key components within the StudyMate platform, illustrating how users interact with study groups, group activities, general resources, and the ranking system based on their interests. while also outlining the role and responsibilities of the system admin in managing the platform and ensuring security.

**User:**

Users of StudyMate, upon creating an account or logging in, gain access to various features. They can join existing study groups or create new ones based on their interests. Within these study groups, users can engage in group activities such as leaving comments, posts, likes, and questions, participating in group chats, uploading materials, and accumulating points for ranking groups. Additionally, users have access to general resources, where they can make use of resources like images, text, files, etc., and contribute by uploading additional resources. 

**Interest:**

User interests will help the system recommend users study groups to join and resources from the general library to explore, enhancing their overall experience on the platform.
Study Group:
Study groups serve as collaborative spaces for users with shared interests or academic pursuits. Users can join existing groups or create new ones, facilitating collective learning and collaboration.

**Group Activities:**

Within study groups, users can engage in various activities to facilitate learning and interaction. These activities include leaving comments, posts, likes, and questions, participating in group chats, and uploading educational materials to share with other groups or group members. Apart from that, there's an additional activity which is the ranking of the study groups. Study groups are ranked based on the points accumulated by their contributions to the general library. 

**Points:**

The system calculates the total points accumulated by all users within a group to determine its ranking. Ranking assigns points to the group of user according to the amount of likes given by other group members to their posts or the resources they uploaded into the General Library (that depends mostly on quality and quantity), fostering healthy competition and incentivizing active participation. 

**General Library Resources:**

The General Library is a repository of resources accessible to all users who are in a study group within StudyMate. Users can access and utilize resources available in the library and contribute by uploading additional materials, thereby enriching the collective knowledge base of the platform.

**Admin:**

The system admin holds additional permissions and responsibilities compared to regular users. 
The system admin is tasked with managing various aspects of the platform, including content moderation, group management, and user account administration(managing user profiles/accounts by handling tasks such as creating, deleting, and resetting passwords). They have the authority to create, edit, and delete study groups as needed, ensuring the platform remains organized and conducive to learning.
Ensuring the security and integrity of the platform is a key responsibility of the system admin. They are responsible for monitoring content for inappropriate behavior, taking measures to address reports from users, and implementing security protocols to safeguard the platform and its users from potential threats or breaches.

## Use case Diagrams
![StudyMate_UseCase-UseCase_User](https://github.com/MetaKt/StudyMate/assets/131533232/7601017b-90b1-4da0-aca8-9d008ffc86b7)

<p align = "center"> Figure UseCase Diagram for User </p>

The Use Case Diagram depicts the features an actor is capable of accessing. For our StudyMate Use Case Diagram, it is separated into two distinct diagrams for ease of comprehension. Figure 3.1.1 above is the Use Case Diagram for Users, representing all the actions a user can perform in the StudyMate platform: Sign Up, Login, Join Group, Join Private Group, Create Group, Post, Like Post, Share Post, Browse General Library, Upload Resources, Share Resources, Edit Profile, and Edit Group. 

**Sign Up and Login:**

Before accessing the StudyMate platform, every user must verify themselves. First-time user must first sign up to the platform, creating their account with a unique username, sophisticated password, and interesting bio description. Then, they will have to verify themselves through our authentication methods and select to join at least one interested study group. For users who already have an account, they will need to log in with their respective usernames and password. Only when given the correct username and password, the user can access the platform and services.

**Join Group, Join Private Group and Create Group:**

Join Group is an action when users are desiring to enter other study groups apart from which they are already a member. A list of available groups will be provided based on the Recommendation feature, an algorithm that will select groups or resources according to the user's interest. Users will then be able to decide to join any group type: Protected or Private Groups. Protected Groups are groups which their content can be only visible to non-member users, giving a better image of the group community. Private Groups are groups that only group members can see through their content within the group, allowing more privacy to the group members. Upon clicking join group, users will from the moment become a member of the group they desire to enter, capable of all group members' services. Unlike protected, before being a member of a private group, the head of the private group must first accept joining private group requests from the user. Only the accepted request can give the user permission to entry and become a group member.

**Post:**

StudyMate provides a space for the group community to post information in the group. A Post can be text, images, videos, or file documents (**list**). A post is a place aiming to encourage communication within the group, producing an active and lively group study environment. Many benefits group members can gain advantage from posts. For example, making a real-life meet-up between group members through posts, sharing information related to the group's content, and discussing a certain topic as one. 

**Like Post and Share Post:**

Within a group, there will appear posts provided by the group members. When a user who is one of the group members sees a post, he/she can like the post to participate in encouraging group study. Liking a post will also be counted as one of the factors to increase the group points for the Ranking System, leading to more group exposure and reputation.

Apart from liking, a user who is one of the group members can also share the post with another group he/she is currently a part of as well. This will create more interactions, not just within one group, but as well as other groups with the same interest and goals.

Our aim is to encourage and increase the capability of group study to its finest. Having these two features will help us in achieving the ideal community.


**Browse General Library:**

The General Library is our system's core feature. It is a huge library where every user can access to it services through any study group. This library provides a common and general ground for all the groups with all interests to showcase and share their resources with the StudyMate community. Likewise library in real life, not only you can browse and research for resources corresponding to your interests, but a user can request to add their own outer resource into the library, and can share their interested resources with the groups as well. Resources in the General Library can be in any form of information as long as it is verified and informative for our community.

**Upload Resources:**

Continuing from the above paragraph, a user is capable of giving their own resource of information to the General Library. Once a user provides their own resource, it will then first be sent to our administrator to check the content for verification and security. The requested-to-upload resource will only appear in the General Library after it has been checked by the administrator. 

**Share Resources:**

As mentioned previously, in the General Library, a resource can be shared to other groups. This provides a way to share information with the group study and promote more research within the study group.

**Edit Profile:**

A user must provide their information and descriptions upon their sign-up stage. However, our system is not limited to only that. A user is free to change the information in their profile according to their satisfaction and desire, as long as it is not offending to other users in the community.

**Edit Group:**

Similar to as User Profile, a group name and description can be changed according to the group members' satisfaction and desire, as long as it is not offending to other users in the community. However, only the group leader is capable of doing so.

![StudyMate_UseCase-UseCase_Admin](https://github.com/MetaKt/StudyMate/assets/131533232/5c6ebfdd-5fa1-4910-afb0-d5ce1e50437a)
<p align = "center"> Figure UseCase Diagram for Admin </p>

The Diagram above, Figure Figure 3.1.2, is the Use Case Diagram for the Administrator, representing all the actions an admin can perform in the StudyMate platform: Check Profile, Check Post, Check Library Resources, User/Group Management, Detect Inappropriate Behaviour, Click Help, and Send Report.

**Check Profile**

An administrator can run through each user's profile to check their information for safety and security concerns, keeping a nice, welcoming, and warm community that will encourage group study further more.

**Check Post**

Same as Check Profile, posts within the group must also be supervised by the administrator. Detecting threats, and harmful, inappropriate, violent, and false information is the duty of the administrator.

**Check Library Resources**
Another important feature of our platform is the General Library, where the information given there must be correct and legitimate. Before a resource provided by a user appears in the General Library, it must be checked thoroughly by the administrator. The administrator must check the content, wording, and other legitimate requirements, in order to prevent copyright, crimes, and false information.

**User/Group Management**

The administrator have the full ability to move/kick any users from the groups/platform, depending on the seriousness of the case. This will help maintain a peaceful environment for focusing on group study encouragement.

**Detect Inappropriate Behaviour**

Another duty of the administrator is to detect inappropriate behaviors in the platform. Then, the administrator can take action on it depending on the seriousness of the case. Moreover, when a user sends a report, the administrator must also come to detect inappropriate behavior verify that the accusation from the user report is true, and take action on it.

**Click Help**

In case of any query from the user of our platform, a user can use the help function to call for help from the administrator. This use case is special because it connects both the users and administrator, as these two actors can contribute to this function. When a user clicks help, this will notify the administrator, and they will acknowledge the situation.

**Send Report**

This use case is used by the user. It is also an extension of the Detect Inappropriate Behaviour use case. When a user spot suspicious behavior that may lead to the unsafety of the community, they can send a report to the administrator for further inspection. Therefore, this use case is linked with the Detect Inappropriate Behaviour use case.




## 2 Structural Modeling
In this chapter, we will see the System Design of the StudyMate software modeling and requirement document. In this section, we delve into the architectural blueprint of StudyMate, a revolutionary platform tailored to enhance the educational experience for students and educators alike.

In this chapter, we will elucidate the architectural components, data flow mechanisms, and interaction protocols that underpin StudyMate’s functionality. By exploring the system’s design rationale, you will gain insights into the foundational principles guiding its development and evolution.

Our approach to system design is rooted in modularity, extensibility, and maintainability, ensuring that StudyMate can adapt to evolving educational paradigms and technological advancements. Through comprehensive architectural diagrams, interface specifications, and design patterns, we aim to provide below a comprehensive roadmap for stakeholders involved in the development and utilization of StudyMate.




## 2.1 Class Diagram

![class Diagram](https://github.com/MetaKt/StudyMate/assets/91473477/f5f5d3be-db91-4984-a926-c38cd36a15bc)

<p align = "left"> Figure 2.1.1 Class Diagram </p>

**Relationships**
<br>
<br>- **User** has <span style="color: green;">Interest.</span>
<br>- **User** joins <span style="color: green;">StudyGroup.</span>
<br>- **StudyGroup** has <span style="color: green;">GroupActivity.</span>
<br>- **User** performs <span style="color: green;">GroupActivity.</span>
<br>- **StudyGroup** accesses <span style="color: green;">GeneralResource.</span>
<br>- **GeneralResource** uploaded by <span style="color: green;">User.</span>
<br>- **Admin** manages <span style="color: green;">User, StudyGroup, GeneralResource, and GroupActivity.</span>
<br><br>
**Notes:**
<br>
<br>- **User** class is the central entity where users can perform various activities related to study groups and resources.
<br>- **Admin** inherits from User, with additional responsibilities and methods.
<br>- Relationships indicate how different classes interact with each other, such as users joining study groups and uploading resources.
<br>- **GroupActivity** and GeneralResource classes capture the specific activities and resources within the platform.
<br>- **Points** system tracks the contributions of users and study groups for ranking purposes.



## 2.2 Package Diagram

![StudyMate_Package](https://github.com/MetaKt/StudyMate/assets/131533232/7628ea59-3e5e-4b3f-8f50-bd3e5aff0962)


<p align = "left"> Figure 2.2.1 Package Diagram </p>

A package diagram is a type of structural diagram in the Unified Modeling Language (UML) used to depict the organization and dependencies between packages or namespaces in a system. Moreover, it is also a valuable tool for visualizing and organizing the structure of a software system, facilitating communication among stakeholders, and supporting software development activities such as design, implementation, and maintenance.


## 2.3 Component Diagram

![component Diagram ](https://github.com/MetaKt/StudyMate/assets/91473477/3939c593-ea56-4f8a-9e00-0413ceb2ada4)


<p align = "left"> Figure 2.3.1 Component Diagram </p>


## 2.4 Deployment Diagram

![StudyMate_DeploymentDiagram](https://github.com/MetaKt/StudyMate/assets/131533232/25473e82-83c8-4615-844a-4fca816c2d13)

<p align = "left"> Figure 2.4.1 Deployment Diagram </p>





## 3 Behavior Modeling


## 3.1 System Sequence Diagram

The System Sequence Diagram illustrates how objects interact in a particular scenario of a system within the StudyMate platform, illustrates how users interact with study groups, group activities, the general library, and the ranking system, and shows communication among stakeholders to provide a clear and concise depiction of the system's behavior, helping stakeholders to understand and discuss the system's functionality and requirements.

In our project, we will separate the System Sequence Diagram into two sections including the user and the admin section.

<i>**Sign Up (For User):**</i>
<br>
<br>
![StudyMate-Sign Up (For Users)](https://github.com/MetaKt/StudyMate/assets/147230981/b5505483-74e3-48c9-a435-2e263fa42a33)
<p align = "left"> Figure 3.1.1 System Diagram Sign Up (For User) </p>
<br>
This part shows the sign-up process, as soon as the new users arrived at the application, the system required them to sign up in order to create an account. When they click “Sign Up”, the system will request the information and the users need to submit the required information. Later on, the system needs to verify that the users are real humans by sending a CAPTCHA test, and after completing it, it will report the account created successfully and bring it to another page to let the users choose groups and show posting resources.
<br>
<br>

<i>**Log In (For User):**</i>
<br>
<br>
![StudyMate-Log In (For Users)](https://github.com/MetaKt/StudyMate/assets/147230981/f028eaf0-eeb3-4eb5-94fb-bc27c8ae41e9)
<p align = "left"> Figure 3.1.2 System Diagram Log In (For User) </p>
<br>
This part shows the sign-up process, as soon as the new users arrived at the application, the system required them to sign up in order to create an account. When they click “Sign Up”, the system will request the information and the users need to submit the required information. Later on, the system needs to verify that the users are real humans by sending a CAPTCHA test, and after completing it, it will report the account created successfully and bring it to another page to let the users choose groups and show posting resources.
<br>
<br>

<i>**Join Group (For User):**</i>
<br>
<br>
![StudyMate-Join Group (For Users)](https://github.com/MetaKt/StudyMate/assets/147230981/8d40e18d-04b9-430a-9dda-4de4870ee3e1)
<p align = "left"> Figure 3.1.3 System Diagram Join Group (For User) </p>
<br>
In this section, it is about showing how to join a group. When the users are interested in any groups, they can just kindly click on the join group button, the system will automatically update the data and report the join group successfully.
<br>
<br>

<i>**Join Private Group (For User):**</i>
<br>
<br>
![StudyMate-Join Private Group (For Users)](https://github.com/MetaKt/StudyMate/assets/147230981/f4b45494-80bc-4a19-86ae-87800577d25e)
<p align = "left"> Figure 3.1.4 System Diagram Join Private Group (For User) </p>

![StudyMate_Contracts](https://github.com/MetaKt/StudyMate/assets/131533232/109b566a-35a8-4f70-91da-20a3a10f1518)


<br>
This diagram illustrates the process of how the user will be able to join a private group. Firstly, the user shall click the join group button which will send the signal to the system and the system will report the joining request to the group leader. Then the next process is the process of “Request Consideration”. If the group leader accepts the new user, the leader will click accept a request and the system will update data and send the join group successfully back to the user. However, if the group host clicks decline, the system will report the join group failure to the user.
<br>
<br>

<i>**Create Group (For USer):**</i>
<br>
<br>
![StudyMate-Create Group (For Users)](https://github.com/MetaKt/StudyMate/assets/147230981/36be5226-8697-4fc4-90c6-7f87e2a20b01)
<p align = "left"> Figure 3.1.5 System Diagram Create Group (For User) </p>
<br>
This diagram depicts the topic of how the user can create a group. Firstly, the user must click the “Create group” button then set up the group name and group description and send it to the system. Later on, the system will update the data of a new group will be created and the user’s new group will show the user that his or her new group is already created.
<br>
<br>

<i>**Browse General Library (For User):**</i>
<br>
<br>
![StudyMate-Browse General Library (For Users))](https://github.com/MetaKt/StudyMate/assets/147230981/7d6c479a-f395-481c-b048-1f1c28d2c3a6)
<p align = "left"> Figure 3.1.6 System Diagram Browse General Library (For User) </p>
<br>
This diagram illustrates the concept of “Browse General Library”. So if the users would like to browse resources in the General Library, they must click the button to enter General Library, and the system will bring them to the library and show resources.
<br>
<br>

<i>**Share Resources From General Library (For User):**</i>
<br>
<br>
![StudyMate-Share Resource from General Library (For User)](https://github.com/MetaKt/StudyMate/assets/147230981/3a3bd72d-3d24-4cbc-8d3c-585364154ed0)
<p align = "left"> Figure 3.1.7 System Diagram Share Resources From General Library (For User) </p>
<br>
The diagram above shows the concept of how the users can share resources from the General Library. This is a method of how the users can share resources from the General Library to the groups. First of all, the users should enter General Library and the system will show resources in General Libray to the users. After that, the users click share resources and the system will request the destination to share resources. After the user provides the destination, the system will send the information to the group and show the users that the resource has been shared successfully.
<br>
<br>

<i>**Share Post (For User):**</i>
<br>
<br>
![StudyMate-Share Post (For Users)](https://github.com/MetaKt/StudyMate/assets/147230981/006701aa-3355-4b02-8e04-a614da26a481)
<p align = "left"> Figure 3.1.8 System Diagram Share Post (For User) </p>
<br>
The diagram above shows the concept of how users can share posts. This is a method of how the users can share posts from themselves to the General Library. First of all, the users should enter General Library and the system will show resources in General Libray to the users. After that, the users click share post  and the system will request posting resources. After the user provides the resources already, the system will update the information to show the users that the resource has been posted successfully.
<br>
<br>

<i>**Like Post (For User):**</i>
<br>
<br>
![StudyMate-Like Post (For Users)](https://github.com/MetaKt/StudyMate/assets/147230981/8b5d60af-e5c7-4d34-9375-115c84712ff0)
<p align = "left"> Figure 3.1.9 System Diagram Like Post (For User) </p>
<br>
In this diagram, it provides the concept of liking posts. As soon as the users enter a group and see the post that they like, they will click the like button and the system will update the data. Then the system will update like to the group and the group will show like to the users.
<br>
<br>

<i>**Post In Group (For User):**</i>
<br>
<br>
![StudyMate-Post in Group  (For Users)](https://github.com/MetaKt/StudyMate/assets/147230981/f22dcaae-c1d0-4104-ab3e-dfe626580b47)
<p align = "left"> Figure 3.1.10 System Diagram Post In Group (For User) </p>
<br>
In this diagram, it shows the process of how the users will post in a group. Firstly, the users must enter the group and then click the “Create post” button. Later on, the system will ask the users to provide resources. After the users provide resources, the system will update the data and show posts in the gro
<br>
<br>

<i>**Edit Profile (For User):**</i>
<br>
<br>
![StudyMate-Edit Profile (For Users)](https://github.com/MetaKt/StudyMate/assets/147230981/fa46fd68-ca8c-4120-8bc4-fd4e8f3468c4)
<p align = "left"> Figure 3.1.11 System Diagram Edit Profile (For User) </p>
<br>
This diagram reveals how to edit profile information, the users must go to their profile page after that the system sends back the requested information and shows information to the users. Then the users click the edit profile button and can start editing their profile information. After finishing the system will update the data send new profile information to the profile page and show it to the users.
<br>
<br>

<i>**Edit Group (For User):**</i>
<br>
<br>
![StudtMate-Edit Group (For Users)](https://github.com/MetaKt/StudyMate/assets/131533232/2649c6d1-94a1-4d24-aa9a-af003bcdf625)

<p align = "left"> Figure 3.1.12 System Diagram Edit Group (For User) </p>

![StudyMate_Contracts](https://github.com/MetaKt/StudyMate/assets/131533232/2df7980f-ce0b-475d-ae23-a9f933fb7d7b)


<br>
This diagram reveals how to edit the group's information, the users must go to the group page and the system will send back the group's information. After that, the user can click the edit group information button. However, the person who could edit the group's information must be the group's leader only, therefore, the system needs to verify whether the user is the leader by sending verification. If the user passes the verification, the system will allow them to update the information, update new information, and show new group information to the user. If the user does not pass the verification, the system will report verification failure to the user.
<br>
<br>

<i>**Check Post (For Admin):**</i>
<br>
<br>
![StudyMate-Check Post (For Admin)](https://github.com/MetaKt/StudyMate/assets/147230981/15508c06-f050-40ad-b675-b4cc6e0d491c)
<p align = "left"> Figure 3.1.13 System Diagram Check Post (For Admin) </p>
<br>
This diagram shows the process of checking the posting of admin. Firstly, the admin will request a post from the system to check then the system will show the requested posts to the admin and the admin can check the post..
<br>
<br>


<i>**Check Library Resources (For Admin):**</i>
<br>
<br>
![StudyMate-Check Library Resouces  (For Admin)](https://github.com/MetaKt/StudyMate/assets/147230981/fb8adb8c-23d1-4c7a-96b0-77b9aafd7241)
<p align = "left"> Figure 3.1.14 System Diagram Check Post (For Admin) </p>
<br>
This diagram shows the process of checking the posting of admin. Firstly, the admin will browse resources in the general Library to check then the system will show the posts to the admin. Later on, the admin can check the post.
<br>
<br>

<i>**Come Help (For Admin):**</i>
<br>
<br>
![StudyMate-Come help (For Admin)](https://github.com/MetaKt/StudyMate/assets/147230981/cb9ad22b-ceb9-4d90-8276-2f111337ec40)

<p align = "left"> Figure 3.1.15 System Diagram Come Help (For Admin) </p>
<br>
This diagram depicts how the admin can come and help the users. Firstly, the users must click the help button which will send a signal to the system, and the system will report to the admin that there is a user who needs help. So, the admin can go and fix the problem of the users.
<br>
<br>

<i>**Detect Inappropriate Behavior (For Admin):**</i>
<br>
<br>
<br>
![StudyMate-Detect Inappropriate Behavior (For Admin)](https://github.com/MetaKt/StudyMate/assets/147230981/5d0a9f0b-957b-4aa7-ba6f-7fedc1b46d6d)
<p align = "left"> Figure 3.1.16 System Diagram Detect Inappropriate Behavior (For Admin) </p>
<br>
This diagram shows how the admin can take action with inappropriate behavior. First of all, when the users see any inappropriate behavior, they can click report and the signal will be sent to the system. After that, the system will tell the admin that there is suspicious behavior and the admin can take action with that suspicious behavior.
<br>
<br>


## 3.2 Sequence Diagram
A sequence diagram is a type of Unified Modeling Language (UML) diagram that is used to model the dynamic behavior of a system by depicting the sequence of messages exchanged between objects or components.

In our project, we will separate the Sequence Diagram into two sections including the user and the admin section.

<i>**Sign Up (For Users):**</i>
<br>
<br>
![Sequence Diagram-Sign Up (For Users)](https://github.com/MetaKt/StudyMate/assets/147230981/be69a126-453b-4aa1-ad8a-015f2276b973)

<p align = "left"> Figure 3.2.1 Sequence Diagram Sign Up (For Users) </p>
<br>
<br>

<i>**Log In (For Users):**</i>
<br>
<br>
![Sequence Diagram-Log In (For Users)](https://github.com/MetaKt/StudyMate/assets/147230981/d33a6472-b329-4216-858a-1bc71f4e7f43)
<p align = "left"> Figure 3.2.2 Sequence Diagram Log In (For Users) </p>
<br>
<br>

<i>**Join Group (For Users):**</i>
<br>
<br>
![Sequence Diagram-Join Group (For Users)](https://github.com/MetaKt/StudyMate/assets/147230981/7f4f22e9-5e91-41ed-a890-e1a9ee4f2cc8)
)
<p align = "left"> Figure 3.2.3 Sequence Diagram Join Group (For Users) </p>
<br>
<br>

<i>**Join Private Group (For Users):**</i>
<br>
<br>
![Sequence Diagram-Join Private Group (For Users)](https://github.com/MetaKt/StudyMate/assets/147230981/82f5b2b0-1f50-4acb-8e26-88812ae075f1)

<p align = "left"> Figure 3.2.4 Sequence Diagram Join Private Group (For Users) </p>
<br>
<br>

<i>**Create Group (For Users):**</i>
<br>
<br>
![Sequence Diagram-Create Group (For Users) (1)](https://github.com/MetaKt/StudyMate/assets/147230981/8bd39044-cda3-4923-a4f5-20152d6d96e1)

<p align = "left"> Figure 3.2.5 Sequence Diagram Create Group (For Users)
<br>
<br>

<i>**Browse General Library (For Users):**</i>
<br>
<br>
![Sequence Diagram-Browse General Library (For Users)](https://github.com/MetaKt/StudyMate/assets/147230981/68dd570a-05a9-425f-9f0f-db39237d5053)

<p align = "left"> Figure 3.2.6 Sequence Diagram Browse General Library (For Users)
<br>
<br>

<i>**Share Resource from General Library (For Users):**</i>
<br>
<br>
![Sequence Diagram-Share Resource from General Library (For Users)](https://github.com/MetaKt/StudyMate/assets/147230981/56d1e370-9a65-47a4-8dc5-772e87afa9d5)

<p align = "left"> Figure 3.2.7 Sequence Diagram Share Resource from General Library (For Users)
<br>
<br>

<i>**Share Post (For Users):**</i>
<br>
<br>
![Sequence Diagram-Share Post (For Users)](https://github.com/MetaKt/StudyMate/assets/147230981/b0794d35-d9bf-4c97-9d62-264680dce89c)

<p align = "left"> Figure 3.2.8 Sequence Diagram Share Post (For Users)
<br>
<br>

<i>**Like Post (For Users):**</i>
<br>
<br>
![Sequence Diagram-Like Post (For Users)](https://github.com/MetaKt/StudyMate/assets/147230981/331c3d26-5ed7-4e74-91b8-0bb166805f31)
<p align = "left"> Figure 3.2.9 Sequence Diagram Like Post (For Users)
<br>
<br>

<i>**Post In Group (For Usesr):**</i>
<br>
<br>
![Sequence Diagram-Post in Group (For Users)](https://github.com/MetaKt/StudyMate/assets/147230981/9280f6ab-cb40-48fb-a6ab-e6bc1862082c)

<p align = "left"> Figure 3.2.10 Sequence Diagram Post In Group (For Users)
<br>
<br>
![Sequence Diagram-Edit Group (For Users)](https://github.com/MetaKt/StudyMate/assets/147230981/f86f3645-6d69-4b4d-822e-8bb2ff39f3b9)

<i>**Edit Profile (For Users):**</i>
<br>
<br>
![Sequence Diagram-Edit Profile (For Users)](https://github.com/MetaKt/StudyMate/assets/147230981/9cb4daa0-a54b-42e6-b3f2-a1136d39f926)

<p align = "left"> Figure 3.2.11 Sequence Diagram Edit Profile (For Users)
<br>
<br>

<i>**Edit Group (For Users):**</i>
<br>
<br>
![Sequence Diagram-Edit Group (For Users)](https://github.com/MetaKt/StudyMate/assets/147230981/b50da5a7-40e2-4620-9863-ca192105ee84)
<p align = "left"> Figure 3.2.12 Sequence Diagram Edit Group (For Users)
<br>
<br>

<i>**Manage Content (For Admin):**</i>
<br>
<br>
![Sequence Diagram-Manage Content (For Admin)](https://github.com/MetaKt/StudyMate/assets/147230981/1151fa21-ddda-4eee-a2df-060c55839a5f)
<p align = "left"> Figure 3.2.13 Sequence Diagram Manage Content (For Admin)
<br>
<br>

<i>**Manage Library Resource (For Admin):**</i>
<br>
<br>
![Sequence Diagram-Manage Library Resource (For Admin)](https://github.com/MetaKt/StudyMate/assets/147230981/fff4327a-0a84-4f78-afc0-609456cd0f2a)
<p align = "left"> Figure 3.2.14 Sequence Diagram Manage Library Resource (For Admin)
<br>
<br>
 
![Sequence Diagram-Click Help (For Admin)](https://github.com/MetaKt/StudyMate/assets/147230981/684acc3e-58b2-4825-addd-107186b825e2)

<p align = "left"> Figure 3.2.15 Sequence Diagram Click Help (For Admin)
<br>
 
<i>**Monitor Security (For Admin):**</i>
<br>
<br>
![Sequence Diagram-Monitor Security (For Admin)](https://github.com/MetaKt/StudyMate/assets/147230981/2bb4f157-30da-42ea-b6d2-3eaef6574894)
<p align = "left"> Figure 3.2.16 MOnitor Security Sequence Diagram Click Help (For Admin)
<br>
<br>


## 3.3 State Machine Diagram
A state machine diagram, also known as a state diagram or state transition diagram, is a graphical representation of a system's behavior that models the different states the system can be in, as well as the transitions between those states.

<br>
![State Machine Diagram-Log In](https://github.com/MetaKt/StudyMate/assets/147230981/564215c2-c1ab-4638-8374-3c36595945b9)
<p align = "left"> Figure 3.3.1 State Machine Diagram (Log In)</p>
<br>

<br>
![State Machine Diagram-Sign Up](https://github.com/MetaKt/StudyMate/assets/147230981/1f5a6bba-8733-4251-ab4e-51ec55483beb)
<p align = "left"> Figure 3.3.2 State Machine Diagram (Sign Up)</p>
<br>

<br>
![State Machine Diagram-Browse General Library](https://github.com/MetaKt/StudyMate/assets/147230981/ea0bfa17-9bf2-4045-bae5-02a82a7efb28)
<p align = "left"> Figure 3.3.3 State Machine Diagram (Group Joining)</p>
<br>

<br>
![State Machine Diagram-Group Joining](https://github.com/MetaKt/StudyMate/assets/147230981/e0c09c88-6e6a-4fce-965c-57f0f85897ea)
<p align = "left"> Figure 3.3.4 State Machine Diagram (Browse General Library)</p>
<br>

<br>
![State Machine Diagram-Upload Resources](https://github.com/MetaKt/StudyMate/assets/147230981/497ef00e-5158-44f6-a9bf-2c65e53226e4)
![Sequence Diagram-Browse General Library (For Users)](https://github.com/MetaKt/StudyMate/assets/147230981/00fc1649-ed40-4e6d-baad-dd2d4f6af0f2)

<p align = "left"> Figure 3.3.5 State Machine Diagram (Upload Resources)</p>
<br>

<br>
<br>


## 3.4 Activity Diagram for Major Use Cases
An activity diagram is a type of Unified Modeling Language (UML) diagram that is used to model the flow of activities or actions within a system or a business process
<br>

![StudyMate_ActivityDiagrams-Page-1](https://github.com/MetaKt/StudyMate/assets/131533232/17560f70-04f0-46ed-b7b0-580b04209653)


<p align = "left"> Figure 3.4.1 Activity Diagram (Browse General Library & Group Joining) </p>

![StudyMate_ActivityDiagrams-Page-2](https://github.com/MetaKt/StudyMate/assets/131533232/d2fe9f3a-2380-485c-87dc-42e074a303ad)


<p align = "left"> Figure 3.4.2 Activity Diagram (Upload Resource & Sign Up) </p>

![StudyMate_ActivityDiagrams-Page-3](https://github.com/MetaKt/StudyMate/assets/131533232/60f6e48b-df38-4900-9b1d-eab8ae26a98d)


<p align = "left"> Figure 3.4.3 Activity Diagram (Click Help) </p>
<br>
<br>


