# StudyMate
This is a project made by Wuhan University International Students of the year 2022 for the Requirement and Modeling class. 
The project's objective is required to complete a requirement document for a system introduced by the students. 

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

##  1 Introduction
As the landscape of education evolves, students encounter new challenges in their learning journey. The increasing complexity of academic subjects, coupled with the need for collaborative learning in today's fast-paced world, has prompted the development of StudyMate. Recognizing the difficulties students face in finding suitable study groups, sharing knowledge effectively, and 
fostering a sense of community, StudyMate aims to bridge these gaps. By providing an interactive platform that facilitates group study, knowledge exchange, and community building, StudyMate 
strives to enhance the overall learning experience for students in universities and beyond.
In this document we will see the different software modelings and how they are modeled. Furthermore, we will look at the purpose, intended audience, and scope of this document and project.

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

## 1.4 Document Overview






## 2 Overall description




## 3 Specific requirements




## 4 System design
In this chapter, we will see the System Design of the StudyMate software modeling and requirement document. In this section, we delve into the architectural blueprint of StudyMate, a revolutionary platform tailored to enhance the educational experience for students and educators alike.

In this chapter, we will elucidate the architectural components, data flow mechanisms, and interaction protocols that underpin StudyMate’s functionality. By exploring the system’s design rationale, you will gain insights into the foundational principles guiding its development and evolution.

Our approach to system design is rooted in modularity, extensibility, and maintainability, ensuring that StudyMate can adapt to evolving educational paradigms and technological advancements. Through comprehensive architectural diagrams, interface specifications, and design patterns, we aim to provide below a comprehensive roadmap for stakeholders involved in the development and utilization of StudyMate.

## 4.1 Domain model
![StudyMate_Domain Model](https://github.com/MetaKt/StudyMate/assets/91473477/a0d0d9b0-3c8e-4f9e-9524-babb4306e049)

 Figure 4.1.1 Logical Structural View: Domain Model Diagram </p>

The domain model provides an abstract, high-level overview of the key components within the StudyMate platform, illustrating how users interact with study groups, group activities, general resources, and the ranking system based on their interests. while also outlining the role and responsibilities of the system admin in managing the platform and ensuring security.

**User:**

Users of StudyMate, upon creating an account or logging in, gain access to various features. They can join existing study groups or create new ones based on their interests. Within these study groups, users can engage in group activities such as leaving comments, posts, likes, and questions, participating in group chats, uploading materials, and accumulating points for ranking groups. Additionally, users have access to general resources, where they can make use of resources like images, text, files, etc., and contribute by uploading additional resources. 

**Interest:**

User interests will help the system recommend users study groups to join and resources from the general library to explore, enhancing their overall experience on the platform.
Study Group:
Study groups serve as collaborative spaces for users with shared interests or academic pursuits. Users can join existing groups or create new ones, facilitating collective learning and collaboration.

**Group Activities:**

Within study groups, users can engage in various activities to facilitate learning and interaction. These activities include leaving comments, posts, likes, and questions, participating in group chats, and uploading educational materials to share with other groups or group members. Apart from that, there's an additional activity that is the ranking of the study groups. Study groups are ranked based on the points accumulated by their contributions to the general library. 

**Points:**

The system calculates the total points accumulated by all users within a group to determine its ranking. Ranking assigns points to the group of user according to the amount of likes given by other group members to their posts or the resources they uploaded into the General Library (that depends mostly on quality and quantity), fostering healthy competition and incentivizing active participation. 

**General Library Resources:**

The General Library is a repository of resources accessible to all users who are in a study group within StudyMate. Users can access and utilize resources available in the library and contribute by uploading additional materials, thereby enriching the collective knowledge base of the platform.

**Admin:**

The system admin holds additional permissions and responsibilities compared to regular users. 
The system admin is tasked with managing various aspects of the platform, including content moderation, group management, and user account administration(managing user profiles/accounts by handling tasks such as creating, deleting, and resetting passwords). They have the authority to create, edit, and delete study groups as needed, ensuring the platform remains organized and conducive to learning.
Ensuring the security and integrity of the platform is a key responsibility of the system admin. They are responsible for monitoring content for inappropriate behavior, taking measures to address reports from users, and implementing security protocols to safeguard the platform and its users from potential threats or breaches.

## 4.2 Use case Diagrams
![StudyMate_UseCase-UseCase_User](https://github.com/MetaKt/StudyMate/assets/131533232/7601017b-90b1-4da0-aca8-9d008ffc86b7)

<p align = "center"> Figure 4.2.1 UseCase Diagram for User </p>

The Use Case Diagram depicts the features an actor is capable of accessing. For our StudyMate Use Case Diagram, it is separated into two distinct diagrams for ease of comprehension. Figure 4.2.1 above is the Use Case Diagram for Users, representing all the actions a user can perform in the StudyMate platform: Sign Up, Login, Join Group, Join Private Group, Create Group, Post, Like Post, Share Post, Browse General Library, Upload Resources, Share Resources, Edit Profile, and Edit Group. 

**Sign Up and Login:**

Before accessing the StudyMate platform, every user must verify themselves. First time user must first signup to the platform, creating their account with a unique username, sophisticated password, and interesting bio description. Then, they will have to verify themselves through our authentication methods and select to join at least one interested study group. For users who already have an account, they will need to login with their respective username and password. Only when given with the correct username and password, the user can access to the platform and services.

**Join Group, Join Private Group and Create Group:**

Join Group is an action when users are desiring to entry other study groups apart from which they are already a member of. A list of available groups will be provided based on the Recommendation feature, an algorithm that will select groups or resources according to the user's interest. Users will then be able to decide to join any group type: Protected or Private Groups. Protected Groups are groups which their content can be only visible to non-member users, giving a better image of the group community. Private Groups are groups that only group members can see through their content within the group, allowing more privacy to the group members. Upon clicking join group, users will from the moment become a member of the group they desire to enter, capable of all group members' services. Unlike protected, before being a member of a private group, the head of the private group must first accept joining private group requests from the user. Only the accepted request can give the user permission to entry and become a group member.

**Post:**

StudyMate provides a space for the group community to post information in the group. A Post can be text, images, videos, or file documents (**list**). A post is a place aiming to encourage communication within the group, producing an active and lively group study environment. Many benefits group members can gain advantage from posts. For example, making a real-life meet-up between group members through posts, sharing information related to the group's content, and discussing a certain topic as one. 

**Like Post and Share Post:**

Within a group, there will appear posts provided by the group members. When a user who is one of the group members see a post, he/she can like the post to participate in encouraging group study. Liking a post will also be counted as one of the factors to increase the group points for Ranking System, leading to more group exposure and reputation.

Apart from liking, a user who is one of the group members can also share the post to another group he/she is currently a part of as well. This will create more interactions, not just within one group, but as well as other groups with the same interest and goal.

Our aim is to encourage and increase the capability of group study to its finest. Having these two features will help us in achieving the ideal community.


**Browse General Library:**

General Library is our system core feature. It is a huge library where every user can access to it services through any study group. This library provides a common and general ground for all the groups with all interests to showcase and share their resources to the StudyMate community. Likewise library in real life, not only you can browse and research for resources corresponding to your interests, a user can request to add their own outer resource into the library, and can share their interested resources to the groups as well. Resources in the General Library can be in any form of information as long as it is verified and informative for our community.

**Upload Resources:**

Continuing from the above paragraph, a user is capability of giving their own resource of information into the General Library. Once a user provided their own resource, it will then first send to our administrator to check the content for verification and security. The requested-to-upload resource will only be appear in the General Library after it has been checked by the administrator. 

**Share Resources:**

As mentioned previously, in the General Library, a resource can be shared to other groups. This provides a way to share information to the group study and promote more research within the study group.

**Edit Profile:**

A user must provide their information and descriptions upon their sign up stage. However, our system is not limited to only that. A user is free to change their information in their profile according to their satisfaction and desire, as long as it is not offending to other users in the community.

**Edit Group:**

Same as User Profile, a group name and description can be changed according to the group members' satisfaction and desire, as long as it is not offending to other users in the community. However, only the group leader is capable of doing so.

![StudyMate_UseCase-UseCase_Admin](https://github.com/MetaKt/StudyMate/assets/131533232/5c6ebfdd-5fa1-4910-afb0-d5ce1e50437a)
<p align = "center"> Figure 4.2.1 UseCase Diagram for Admin </p>

The Diagram above, Figure 4.2.1, is the Use Case Diagram for Administrator, representing all the actions an admin can perform in the StudyMate platform: Check Profile, Check Post, Check Library Resources, User/Group Management, Detect Inappropriate Behaviour, Click Help, and Send Report.

**Check Profile**

An administrator can run through each user's profile to check their information for safety and security concerns, keeping a nice, welcoming, and warm community that will encourage group study further more.

**Check Post**

Same as Check Profile, posts within the group must also be supervised by the administrator. Detecting threats, harmful, inappropriate, violence, and false information is a duty of the administrator.

**Check Library Resources**
Another important feature of our platform is the General Library, where the information given there must be correct and legitimate. Before a resource provided by a user appears on the General Library, it must be checked thoroughly by the administrator. The administrator must check the content, wordings, and other legitimate requirements, in order to prevent copyright, crimes, and false information.

**User/Group Management**

The administrator have the full ability to move/kick any users from the groups/platform, depending on the seriousness of the case. This will help maintaining a peaceful environment for focusing on group study encouragment.

**Detect Inappropriate Behaviour**

Another duty for the administrator is to detect inappropriate behaviours in the platform. Then, the administrator can take actions on it depending on the seriousness of the case. Moreover, when a user send a report, the administrator must also come to detect inappropriate behaviour and verify that the accussion in a user report is true and take actions on it.

**Click Help**

**Send Report**




## 4.3 System Sequence Diagram

The System Sequence Diagram illustrates how objects interact in a particular scenario of a system within the StudyMate platform, illustrates how users interact with study groups, group activities, the general library, and the ranking system, and shows communication among stakeholders to provide a clear and concise depiction of the system's behavior, helping stakeholders to understand and discuss the system's functionality and requirements.

In our project, we will separate the System Sequence Diagram into two sections including the user and the admin section.

<i>**Sign Up (For User):**</i>
<br>
<br>
![StudyMate-Sign Up (For Users)](https://github.com/MetaKt/StudyMate/assets/147230981/b5505483-74e3-48c9-a435-2e263fa42a33)
<p align = "left"> Figure 4.3.1 System Diagram Sign Up (For User) </p>
<br>
This part shows the sign-up process, as soon as the new users arrived at the application, the system required them to sign up in order to create an account. When they click “Sign Up”, the system will request the information and the users need to submit the required information. Later on, the system needs to verify that the users are real humans by sending a CAPTCHA test, and after completing it, it will report the account created successfully and bring it to another page to let the users choose groups and show posting resources.
<br>
<br>

<i>**Log In (For User):**</i>
<br>
<br>
![StudyMate-Log In (For Users)](https://github.com/MetaKt/StudyMate/assets/147230981/f028eaf0-eeb3-4eb5-94fb-bc27c8ae41e9)
<p align = "left"> Figure 4.3.2 System Diagram Log In (For User) </p>
<br>
This part shows the sign-up process, as soon as the new users arrived at the application, the system required them to sign up in order to create an account. When they click “Sign Up”, the system will request the information and the users need to submit the required information. Later on, the system needs to verify that the users are real humans by sending a CAPTCHA test, and after completing it, it will report the account created successfully and bring it to another page to let the users choose groups and show posting resources.
<br>
<br>

<i>**Join Group (For User):**</i>
<br>
<br>
![StudyMate-Join Group (For Users)](https://github.com/MetaKt/StudyMate/assets/147230981/8d40e18d-04b9-430a-9dda-4de4870ee3e1)
<p align = "left"> Figure 4.3.3 System Diagram Join Group (For User) </p>
<br>
In this section, it is about showing how to join a group. When the users are interested in any groups, they can just kindly click on the join group button, the system will automatically update the data and report the join group successfully.
<br>
<br>

<i>**Join Private Group (For User):**</i>
<br>
<br>
![StudyMate-Join Private Group (For Users)](https://github.com/MetaKt/StudyMate/assets/147230981/f4b45494-80bc-4a19-86ae-87800577d25e)
<p align = "left"> Figure 4.3.4 System Diagram Join Private Group (For User) </p>
<br>
This diagram illustrates the process of how the user will be able to join a private group. Firstly, the user shall click the join group button which will send the signal to the system and the system will report the joining request to the group leader. Then the next process is the process of “Request Consideration”. If the group leader accepts the new user, the leader will click accept a request and the system will update data and send the join group successfully back to the user. However, if the group host clicks decline, the system will report the join group failure to the user.
<br>
<br>

<i>**Create Group (For USer):**</i>
<br>
<br>
![StudyMate-Create Group (For Users)](https://github.com/MetaKt/StudyMate/assets/147230981/36be5226-8697-4fc4-90c6-7f87e2a20b01)
<p align = "left"> Figure 4.3.5 System Diagram Create Group (For User) </p>
<br>
This diagram depicts the topic of how the user can create a group. Firstly, the user must click the “Create group” button then set up the group name and group description and send it to the system. Later on, the system will update the data of a new group will be created and the user’s new group will show the user that his or her new group is already created.
<br>
<br>

<i>**Browse General Library (For User):**</i>
<br>
<br>
![StudyMate-Browse General Library (For Users))](https://github.com/MetaKt/StudyMate/assets/147230981/7d6c479a-f395-481c-b048-1f1c28d2c3a6)
<p align = "left"> Figure 4.3.6 System Diagram Browse General Library (For User) </p>
<br>
This diagram illustrates the concept of “Browse General Library”. So if the users would like to browse resources in the General Library, they must click the button to enter General Library, and the system will bring them to the library and show resources.
<br>
<br>

<i>**Share Resources From General Library (For User):**</i>
<br>
<br>
![StudyMate-Share Resource from General Library (For User)](https://github.com/MetaKt/StudyMate/assets/147230981/3a3bd72d-3d24-4cbc-8d3c-585364154ed0)
<p align = "left"> Figure 4.3.7 System Diagram Share Resources From General Library (For User) </p>
<br>
The diagram above shows the concept of how the users can share resources from the General Library. This is a method of how the users can share resources from the General Library to the groups. First of all, the users should enter General Library and the system will show resources in General Libray to the users. After that, the users click share resources and the system will request the destination to share resources. After the user provides the destination, the system will send the information to the group and show the users that the resource has been shared successfully.
<br>
<br>

<i>**Share Post (For User):**</i>
<br>
<br>
![StudyMate-Share Post (For Users)](https://github.com/MetaKt/StudyMate/assets/147230981/006701aa-3355-4b02-8e04-a614da26a481)
<p align = "left"> Figure 4.3.8 System Diagram Share Post (For User) </p>
<br>
The diagram above shows the concept of how users can share posts. This is a method of how the users can share posts from themselves to the General Library. First of all, the users should enter General Library and the system will show resources in General Libray to the users. After that, the users click share post  and the system will request posting resources. After the user provides the resources already, the system will update the information to show the users that the resource has been posted successfully.
<br>
<br>

<i>**Like Post (For User):**</i>
<br>
<br>
![StudyMate-Like Post (For Users)](https://github.com/MetaKt/StudyMate/assets/147230981/8b5d60af-e5c7-4d34-9375-115c84712ff0)
<p align = "left"> Figure 4.3.9 System Diagram Like Post (For User) </p>
<br>
In this diagram, it provides the concept of liking posts. As soon as the users enter a group and see the post that they like, they will click the like button and the system will update the data. Then the system will update like to the group and the group will show like to the users.
<br>
<br>

<i>**Post In Group (For User):**</i>
<br>
<br>
![StudyMate-Post in Group  (For Users)](https://github.com/MetaKt/StudyMate/assets/147230981/f22dcaae-c1d0-4104-ab3e-dfe626580b47)
<p align = "left"> Figure 4.3.10 System Diagram Post In Group (For User) </p>
<br>
In this diagram, it shows the process of how the users will post in a group. Firstly, the users must enter the group and then click the “Create post” button. Later on, the system will ask the users to provide resources. After the users provide resources, the system will update the data and show posts in the gro
<br>
<br>

<i>**Edit Profile (For User):**</i>
<br>
<br>
![StudyMate-Edit Profile (For Users)](https://github.com/MetaKt/StudyMate/assets/147230981/fa46fd68-ca8c-4120-8bc4-fd4e8f3468c4)
<p align = "left"> Figure 4.3.11 System Diagram Edit Profile (For User) </p>
<br>
This diagram reveals how to edit profile information, the users must go to their profile page after that the system sends back the requested information and shows information to the users. Then the users click the edit profile button and can start editing their profile information. After finishing the system will update the data send new profile information to the profile page and show it to the users.
<br>
<br>

<i>**Edit Group (For User):**</i>
<br>
<br>
![StudyMate-Edit Group (For Users)](https://github.com/MetaKt/StudyMate/assets/147230981/b1f8351d-ee11-4735-a422-faf16270f707)
<p align = "left"> Figure 4.3.12 System Diagram Edit Group (For User) </p>
<br>
This diagram reveals how to edit the group's information, the users must go to the group page and the system will send back the group's information. After that, the user can click the edit group information button. However, the person who could edit the group's information must be the group's leader only, therefore, the system needs to verify whether the user is the leader by sending verification. If the user passes the verification, the system will allow them to update the information, update new information, and show new group information to the user. If the user does not passes the verification, the system will report verification failure to the user.
<br>
<br>

<i>**Check Post (For Admin):**</i>
<br>
<br>
![StudyMate-Check Post (For Admin)](https://github.com/MetaKt/StudyMate/assets/147230981/15508c06-f050-40ad-b675-b4cc6e0d491c)
<p align = "left"> Figure 4.3.13 System Diagram Check Post (For Admin) </p>
<br>
This diagram shows the process of checking the posting of admin. Firstly, the admin will request a post from the system to check then the system will show the requested posts to the admin and the admin can check the post..
<br>
<br>

<i>**Check Post (For Admin):**</i>
<br>
<br>
![StudyMate-Check Post (For Admin)](https://github.com/MetaKt/StudyMate/assets/147230981/15508c06-f050-40ad-b675-b4cc6e0d491c)
<p align = "left"> Figure 4.3.14 System Diagram Check Post (For Admin) </p>
<br>
This diagram shows the process of checking the posting of admin. Firstly, the admin will browse posts in the application to check then the system will show the posts to the admin. Later on, the admin can check the post.
<br>
<br>

<i>**Check Library Resources (For Admin):**</i>
<br>
<br>
![StudyMate-Check Library Resouces  (For Admin)](https://github.com/MetaKt/StudyMate/assets/147230981/fb8adb8c-23d1-4c7a-96b0-77b9aafd7241)
<p align = "left"> Figure 4.3.15 System Diagram Check Post (For Admin) </p>
<br>
This diagram shows the process of checking the posting of admin. Firstly, the admin will browse resources in the general Library to check then the system will show the posts to the admin. Later on, the admin can check the post.
<br>
<br>

<i>**Check Library Resources (For Admin):**</i>
<br>
<br>
![StudyMate-Check Library Resouces  (For Admin)](https://github.com/MetaKt/StudyMate/assets/147230981/fb8adb8c-23d1-4c7a-96b0-77b9aafd7241)
<p align = "left"> Figure 4.3.16 System Diagram Check Library Resources (For Admin) </p>
<br>
This diagram shows the process of checking the posting of admin. Firstly, the admin will browse resources in the general Library to check then the system will show the resources to the admin. Later on, the admin can check the resources in the General Library.
<br>
<br>

<i>**User / Group Management (For Admin):**</i>
<br>
<br>
![StudyMate-Check Library Resouces  (For Admin)](https://github.com/MetaKt/StudyMate/assets/147230981/fb8adb8c-23d1-4c7a-96b0-77b9aafd7241)
<p align = "left"> Figure 4.3.17 System Diagram User / Group Management (For Admin) </p>
<br>
This diagram illustrates how the admin can manage users and groups in the application. First, the admin will browse the user’s or group’s information and the system will show them to the admin. After that, the admin will check the user’s and group’s information.
<br>
<br>

<i>**Come Help (For Admin):**</i>
<br>
<br>
![StudyMate-Come help (For Admin)](https://github.com/MetaKt/StudyMate/assets/147230981/cb9ad22b-ceb9-4d90-8276-2f111337ec40)

<p align = "left"> Figure 4.3.18 System Diagram Come Help (For Admin) </p>
<br>
This diagram depicts how the admin can come and help the users. Firstly, the users must click the help button which will send a signal to the system, and the system will report to the admin that there is a user who needs help. So, the admin can go and fix the problem of the users.
<br>
<br>

<i>**Detect Inappropriate Behavior (For Admin):**</i>
<br>
<br>
![StudyMate-Detect Inappropriate Behavior (For Admin)](https://github.com/MetaKt/StudyMate/assets/147230981/5d0a9f0b-957b-4aa7-ba6f-7fedc1b46d6d)
<p align = "left"> Figure 4.3.19 System Diagram Detect Inappropriate Behavior (For Admin) </p>
<br>
This diagram shows how the admin can take action with inappropriate behavior. First of all, when the users see any inappropriate behavior, they can click report and the signal will be sent to the system. After that, the system will tell the admin that there is suspicious behavior and the admin can take action with that suspicious behavior.
<br>
<br>
