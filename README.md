# StudyMate
This is a project made by Wuhan University International Students of the year 2022 for the Requirement and Modeling class. 
The project's objective is required to complete a requirement document for a system introduced by the students. 

## What is StudyMate?
StudyMate is an exceptional interactive website designed exclusively for individuals seeking to engage in group study. With StudyMate, you can easily connect with like-minded individuals by joining or creating study groups, participate or share resources in the
post sessions, as well as engage in the General Library of StudyMate, and even post meeting details to ensure smooth coordination with your study partners.

## Requirement Document File
https://docs.google.com/document/d/1IJ-cV1o2Ka36fiWwwgnNiymw2SvC3ndocS-qIBZWNsw/edit?usp=sharing

## Work Update
| Date | Week | Description |
| :----: | :---: | :------------------------------------: |
| 2/4/2024 | Week 6 | Domain Model, Use Case Model |
| 5/4/2024 | Week 6 | System Sequence Diagrams |
| 16/4/2024 | Week 8 | Domain Model 2.0, Use Case Model 2.0 |

##  1 Introduction
As the landscape of education evolves, students encounter new challenges in their learning journey. The increasing complexity of academic subjects, coupled with the need for collaborative learning in today's fast-paced world, has prompted the development of StudyMate. Recognizing the difficulties students face in finding suitable study groups, sharing knowledge effectively, and 
fostering a sense of community, StudyMate aims to bridge these gaps. By providing an interactive platform that facilitates group study, knowledge exchange, and community building, StudyMate 
strives to enhance the overall learning experience for students in universities and beyond.
In this document we will see the different software modelings and how they are modelled. Futhermore we wil look at the purpose, intended audience and scope of this document and project.

## 1.1 Document purpose
The main purpose of this document is to provide details of the UMLs and software modelings of StudyMate web application which will focus on some main diagrams and patterns used in the modeling of it. The intention of the document is to help audiences related to Studymate web application to understand how the system is modelled, furthermore, it is also intended to show the project consultant the strengths or weaknesses of the system before the team starts detailed designs. Finally, the project consultant and team members could be able to validate whether the web-application meets the expected software modelings.

## 1.2 Project scope
This document aims to provide a platform where university srudents and individuals are allowed to:

-Explore the available study groups for joining.
-Creat or join study groups.
-After joining groups you can participate in the group discussions.
-Participate in the ranking(of study groups).

The website will serve as a productive hub for educational support, foster a community of learners and incentivate the learnin of users with its different activities.

## 1.3 Intended audience
The intended audience for this document includes:
-Project developers
-Project managers
-Project designers
-Project implementers
-Project testers
-Project stakeholders
-Documentation writers

## 1.4 Document overview






## 2 Overall description




## 3 Specific requirements




## 4 System design
In this chapter we will see the System Design of the StudyMate software modeling and requirement document. In this section, we delve into the architectural blueprint of StudyMate, a revolutionary platform tailored to enhance the educational experience for students and educators alike.

In this chapter, we will elucidate the architectural components, data flow mechanisms, and interaction protocols that underpin StudyMate’s functionality. By exploring the system’s design rationale, you will gain insights into the foundational principles guiding its development and evolution.

The Studymate system is mainly separated into 2 systems:
-Users system
-Admin system

Our approach to system design is rooted in modularity, extensibility, and maintainability, ensuring that StudyMate can adapt to evolving educational paradigms and technological advancements. Through comprehensive architectural diagrams, interface specifications, and design patterns, we aim to provide below a comprehensive roadmap for stakeholders involved in the development and utilization of StudyMate.

## 4.1 Domain model
![StudyMate_Domain Model](https://github.com/MetaKt/StudyMate/assets/91473477/f72e3cd6-b504-4b6a-9892-8c3ba020231a)
Figure 4.1.1 Logical Structural View: Domain Model Diagram

The domain model provides an abstract, high-level overview of the key components within the StudyMate platform, illustrating how users interact with study groups, group activities, general resources, and the ranking system based on their interests. while also outlining the role and responsibilities of the system admin in managing the platform and ensuring security.

User:

User of StudyMate, upon creating an account or logging in, gain access to various features. They can join existing study groups or create new ones based on their interests. Within these study groups, users can engage in group activities such as leaving comments, posts, likes, and questions, participating in group chats, uploading materials, and accumulate points for ranking groups. Additionally, users have access to general resources, where they can make use of resources like images, text, files, etc., and contribute by uploading additional resources. 

Interest:

User's interests will help the system recommend users study groups to join and resources from the general library to explore, enhancing their overall experience on the platform.
Study Group:
Study groups serve as collaborative spaces for users with shared interests or academic pursuits. Users can join existing groups or create new ones, facilitating collective learning and collaboration.

Group Activities:

Within study groups, users can engage in various activities to facilitate learning and interaction. These activities include leaving comments, posts, likes, and questions, participating in group chats, and uploading educational materials to share with other groups or group members. Apart from that there's an additional activity that is the ranking of the study groups. Study groups are ranked based on the points accumulated by their contributions to the general library. 

Points:

The system calculates the total points accumulated by all users within a group to determine its ranking. Ranking assigns points to users according to the amount of likes given by other users to the  resources they uploaded (that depends mostly on the quality and quantity), fostering healthy competition and incentivizing active participation. 

General Library Resources:

The general library is a repository of resources accessible to all users who are in a study group within StudyMate. Users can access and utilize resources available in the library and contribute by uploading additional materials, thereby enriching the collective knowledge base of the platform.

Admin:

The system admin holds additional permissions and responsibilities compared to regular users. 
The system admin is tasked with managing various aspects of the platform, including content moderation, group management, and user account administration(managing user profile/accounts by handling tasks such as creating, deleting, and resetting passwords). They have the authority to create, edit, and delete study groups as needed, ensuring the platform remains organized and conducive to learning.
Ensuring the security and integrity of the platform is a key responsibility of the system admin. They are responsible for monitoring content for inappropriate behaviour, taking measures to address reports from users, and implementing security protocols to safeguard the platform and its users from potential threats or breaches.


