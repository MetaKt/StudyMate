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
| 28/4/2024 | Week 10 | System Diagram) |

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
![StudyMate_UseCase-UseCase_User](https://github.com/MetaKt/StudyMate/assets/131533232/0910c18c-4a7b-4e1b-864e-a0fcc8732c8b)

<p align = "center"> Figure 4.2.1 UseCase Diagram for User </p>

The Use Case Diagram depicts the features an actor is capable of accessing. For our StudyMate Use Case Diagram, it is separated into two distinct diagrams for ease of comprehension. Figure 4.2.1 above is the Use Case Diagram for Users, representing all the actions a user can perform in the StudyMate platform: Sign Up, Login, Join Group, Join Private Group, Create Group, Post, Like Post, Share Post, Browse General Library, Upload Resources, Share Resources, Edit Profile, and Edit Group. 

**Sign Up and Login:**

Before accessing the StudyMate platform, every user must verify themselves. First time user must first signup to the platform, creating their account with a unique username, sophisticated password, and interesting bio description. Then, they will have to verify themselves through our authentication methods and select to join at least one interested study group. For users who already have an account, they will need to login with their respective username and password. Only when given with the correct username and password, the user can access to the platform and services.

**Join Group, Join Private Group and Create Group:**

Join Group is an action when users are desiring to entry other study groups apart from which they are already a member of. A list of available groups will be provided based on the Recommendation feature, an algorithm that will select groups or resources according to the user's interest. Users will then be able to decide to join any group type: Protected or Private Groups. Protected Groups are groups which their content can be only visible to non-member users, giving a better image of the group community. Private Groups are groups that only group members can see through their content within the group, allowing more privacy to the group members. Upon clicking join group, users will from the moment become a member of the group they desire to enter, capable of all group members' services. Unlike protected, before being a member of a private group, the head of the private group must first accept joining private group requests from the user. Only the accepted request can give the user permission to entry and become a group member.

**Post:**

StudyMate provides a space for the group community to post information in the group. A Post can be text, images, videos, or file documents (**list**). A post is a place aiming to encourage communication within the group, producing an active and lively group study environment. Many benefits group members can gain advantage from posts. For example, making a real-life meet-up between group members through posts, sharing information related to the group's content, and discussing a certain topic as one. 

**Like Post and Share Post:**

**Browse General Library:**

**Upload Resources:**

**Share Resources:**

**Edit Profile:**

**Edit Group:**

![StudyMate_UseCase-UseCase_Admin](https://github.com/MetaKt/StudyMate/assets/131533232/5c6ebfdd-5fa1-4910-afb0-d5ce1e50437a)
<p align = "center"> Figure 4.2.1 UseCase Diagram for Admin </p>




## 4.3 Sequence diagram

The sequence diagram illustrates how objects interact in a particular scenario of a system within the StudyMate platform, illustrates how users interact with study groups, group activities, the general library, and the ranking system, and shows communication among stakeholders to provide a clear and concise depiction of the system's behavior, helping stakeholders to understand and discuss the system's functionality and requirements.

**Sign Up (For User):**
<br>
<br>
![StudyMate-Sign Up (For Users)](https://github.com/MetaKt/StudyMate/assets/147230981/b5505483-74e3-48c9-a435-2e263fa42a33)
<p align = "left"> Figure 4.3.1 System Diagram Sign Up (For User) </p>
<br>
This part shows the sign-up process, as soon as the new users arrived at the application, the system required them to sign up in order to create an account. When they click “Sign Up”, the system will request the information and the users need to submit the required information. Later on, the system needs to verify that the users are real humans by sending a CAPTCHA test, and after completing it, it will report the account created successfully and bring it to another page to let the users choose groups and show posting resources.
<br>
<br>

**Log In (For User):**
<br>
<br>
![StudyMate-Log In (For Users)](https://github.com/MetaKt/StudyMate/assets/147230981/f028eaf0-eeb3-4eb5-94fb-bc27c8ae41e9)
<p align = "left"> Figure 4.3.2 System Diagram Log In (For User) </p>
<br>
This part shows the sign-up process, as soon as the new users arrived at the application, the system required them to sign up in order to create an account. When they click “Sign Up”, the system will request the information and the users need to submit the required information. Later on, the system needs to verify that the users are real humans by sending a CAPTCHA test, and after completing it, it will report the account created successfully and bring it to another page to let the users choose groups and show posting resources.
<br>
<br>

**Join Group (For User):**
<br>
<br>
![StudyMate-Join Group (For Users)](https://github.com/MetaKt/StudyMate/assets/147230981/8d40e18d-04b9-430a-9dda-4de4870ee3e1)
<p align = "left"> Figure 4.3.3 System Diagram Join Group (For User) </p>
In this section, it is about showing how to join a group. When the users are interested in any groups, they can just kindly click on the join group button, the system will automatically update the data and report the join group successfully.
<br>
<br>


