# Software Requirements Specification for Ted's Quest




Version 1.0







Revision History

| **Date** | **Version** | **Description** | **Author** |
| --- | --- | --- | --- |
| \&lt;dd/mmm/yy\&gt; | \&lt;x.x\&gt; | \&lt;details\&gt; | \&lt;name\&gt; |
|   |   |   |   |
|   |   |   |   |
|   |   |   |   |

# Table of Contents

1. [Introduction](#1-introduction)         
    1. [Purpose](#11-purpose)     
    2. [Scope](#12-scope)     
    3. [Definitions, Acronyms and Abbreviations](#13-definitions-acronyms-and-abbreviations)     
    4. [References](#14-references)     
    5. [Overview](#15-overview)     
2. [Overall Description](#2-overall-description)    
3. [Specific Requirements](#3-specific-requirements)
    1. [Functionality](#31-functionality)
        1. [Functional Requirement One](#311-functional-requirement-one>)        
    2. [Usability  ](#32-Usability)   
        1. [Usability Requirement One](#321-usability-requirement-one>)
    3. [Reliability](#33-reliability)     
        1. [Reliability Requirement One](#331-reliability-requirement-one>)
    4. [Performance](#34-performance)     
        1. [Performance Requirement One](#341-performance-requirement-one>)
    5. [Supportability](#35-supportability)     
        1. [Supportability Requirement One](#351-supportability-requirement-one>)
    6. [Design Constraints](#36-design-constraints)     
        1. [Design Constraint One](#361-design-constraint-one)
    7. [Online User Documentation and Help System Requirements](#37-on-line-user-documentation-and-help-system-requirements)
    8. [Purchased Components](#38-purchased-components)     
    9. [Interfaces](#39-interfaces)     
        1. [User Interfaces ](#391-user-interfaces)          
        2. [Hardware Interfaces](#392-hardware-interfaces)           
        3. [Software Interfaces](#393-software-interfaces)           
        4. [Communications Interfaces](#394-communications-interfaces)           
    10. [Licensing Requirements ](#310-licensing-requirements)    
    11. [Legal, Copyright and Other Notices](#311-legal-copyright-and-other-notices)     
    12. [Applicable Standards](#312-applicable-standards)  
4. [Supporting Information](#4-supporting-information)   

# 1. Introduction

This document describes the **SRS** of the game **Ted's Quest** by **Ted's Entertainment**. 
It includes the purpose, scope, definitions, acronyms, abbrevations, references to other
documents and an overview of the **SRS**.

## 1.1 Purpose

The purpose of this document is to build a hypercasualed game for computer and mobile applications.

## 1.2 Scope

The game is aimed to be enjoyable, fun and to challenge one or many. The application should be free to download from our GitHub-Server. 
In a first step, there is no need to keep an active internet connection. 
In a further step it should be possible to login and require an active internet connection for a global user highscore. 
Also in a first step, the game is a free computer application with one or two manually crafted levels. 
In a further step, the game should be playable on Android smartphones, contain additional manually crafted levels and an infinite mode. 
Then, in a third step of development, there should be automatically crafted levels and a store to purchase clothing and weapons for the player. 
These should be bought with either credits from playing the game or real money. The actual overall scope is defined by use cases.

## 1.3 Definitions, Acronyms, and Abbreviations

OS <ensp> operating system</br>
UCD <ensp> use case diagram</br>
Player <ensp> character in the game</br>
User <ensp> person playing the game</br>

## 1.4 References

<a href="https://hypercasual.wordpress.com/">Blog</a></br>
<a href="https://dhbw-karlsruhe.myjetbrains.com/youtrack/dashboard?id=f29a1b9e-a4f4-4c06-8ad9-c7f0e6cc7e58">YouTrack Documentation</a></br>
<a href="https://github.com/GabrielBalzer/hypercasualgame">General GitHub Repository</a></br>
<a href="https://github.com/GabrielBalzer/hypercasualgame/tree/master/hellocucumber">Cucumber Testing GitHub</a></br>
<a href="https://github.com/GabrielBalzer/tedsquest_documentation/">User Testing</a></br>
<a href="https://github.com/GabrielBalzer/hypercasualgame/tree/master/tedsquest">Source Code Game GitHub</a></br>
<a href="">Documentation Game GitHub</a></br>
<a href="https://github.com/GabrielBalzer/tedsquest_documentation/blob/master/SAD.pdf">SAD</a></br>
<a href="https://github.com/GabrielBalzer/tedsquest_documentation/blob/master/Use-Case_diagram.png">Overall Use-Case Diagram</a></br>

## 1.5 Overview

This section describes the overview on the document. First ther is an overall description.
After, there will be many requirements listed by their belonging. 

# 2. Overall Description

**Product Perspective:**
The user interface is to be on any computer and is not depending on the installed operating system (OS). 
Therefore we need an hardware interface to the mouse and the keyboard.
On Android-based smartphones and tablets we are going to use the display to control the application. 

In both cases, the application is directly installed on the OS. There will be a system interface to the server,
mainly for the global challenging mode. However, the data of singleplayers will also be able to connect to 
the server to save their local data and play in global challenges.

<div align="center"><img src="https://github.com/GabrielBalzer/tedsquest_documentation/blob/master/Use-Case_diagram.png" alt="UCD Ted's Quest" /></div>

**Design and Implementation Constraints:**
There are some contraints regarding the design and the implementation.
For design, there are issues with the format that the Unity Engine accepts. Since the game is aimed to be excecutable on a computer, not a smartphone, the control remains simple by using the keyboard.
Also in a first step of implementation, it is not required to use an active internet connection. All game actions will be local on the computer.
The game is aimed to be installed with a small effort as possible and little disk space requirements.

**User Charactistics:**
Based on the use case diagrams (UCD) the user can check the application's settings like managing 
the account he logged in, change the sound or the appearence or start the game itself. 
By starting the second semester, we will shorten or enlarge the scope.

**Use Cases:**</br>
<ul>
<li><a href = "https://github.com/GabrielBalzer/tedsquest_documentation/blob/master/Use%20Cases/UC_Mainmenu.md">Use Case: Main Menu</a></br></li>
<li><a href = "https://github.com/GabrielBalzer/tedsquest_documentation/blob/master/Use%20Cases/UC_Settings.md">Use Case: Settings</a></br></li>
<li><a href = "https://github.com/GabrielBalzer/tedsquest_documentation/blob/master/Use%20Cases/UC_Storymenu.md">Use Case: Story Menu</a></br></li>
<li><a href = "https://github.com/GabrielBalzer/tedsquest_documentation/blob/master/Use%20Cases/UC_Soundsettings.md">Use Case: Soundsettings</a></br></li>
<li><a href = "https://github.com/GabrielBalzer/tedsquest_documentation/blob/master/Use%20Cases/UC_MoveRight.md">Use Case: Move Right</a></br></li>
<li><a href = "https://github.com/GabrielBalzer/tedsquest_documentation/blob/master/Use%20Cases/UC_Jump.md">Use Case: Jump</a></br></li>
<li><a href = "https://github.com/GabrielBalzer/tedsquest_documentation/blob/master/Use%20Cases/UC_Shoot.md">Use Case: Shoot</a></br></li>
</ul>

**Product Functions:**
The user shall be able to easily install and execute the application. It should also be easy to remote the application again.
The game is aimed to be self-explaining and can be played by an age range from 6 to 100 years. A first requirement is to play it as single user locally.

**Assumptions:**
Ted's Entertainment assumes the starting and ending of the application to be self-explaining since these functions are provided similar to other computer applications.
Also all parts that the Unity Framework provides are assumed to be correct.

# 3. Specific Requirements

<div align="center"><img src="https://github.com/GabrielBalzer/hypercasualgame/blob/master/exchange/project-diagramm.jpg" alt="UCD Ted's Quest" /></div>

## 3.1 Functionality

### 3.1.1 Functional Requirement One - Login

A functional requirement shall be the login account. The user shall be able to choose between 
a new local account or login with his Google account.
This requirement is outdated for the actual scope.

### 3.1.2 Functional Requirement Two - Manage Account

It shall be possible for the user to manage his account. Therefore it shall be possible to 
logout, delete the account or update any personal information.
This requirement is outdated for the actual scope.

### 3.1.3 Functional Requirement Three - Manage Sound

It shall be possible to change the sound from the application to either turn in on or off 
globally.

### 3.1.4 Functional Requirement Four - User Interface

The application shall provide two views, a dark and a light mode.
This requirement is outdated for the actual scope.

### 3.1.5 Functional Requirement Five - About

The application shall provide a short description about the application and its developer team.
It shall also provide some basic help for the user.

### 3.1.6 Functional Requirement Six - Choose a Level

It shall be possible to have a simple overview over the possible levels. Only the actual and 
the previous levels, that have been ended successfully shall always be accessible. Else, if
the previous level has not been ended successfully, the level shall be locked.

### 3.1.7 Functional Requirement Seven - Customization

It shall be possible to customize the main character, the stickman. 
This requirement is outdated for the actual scope.

### 3.1.8 Functional Requirement Eight - Upgrade

It shall be possible to upgrade the weapons and powerups by purchasing objects by both, real 
money and collected coins from the playthrough.
This requirement is outdated for the actual scope.

### 3.1.9 Functional Requirement Nine - Update the Application

The application shall update itself automatically, without user input.
This requirement is outdated for the actual scope.

### 3.1.10 Functional Requirement Ten - Jump

It shall be possible to make the player jump.

### 3.1.11 Functional Requirement Twelve - Move Right

It shall be possible to move right in order to collect coins and avoid obstacles.

### 3.1.12 Functional Requirement Thirteen - Shoot 

It shall be possible to shoot or destroy objects. Objects are boxes. 
In a first integration step there will be only one way to destroy the boxes, by running through them.


## 3.2 Usability

### 3.2.1 Usability Requirement One - Simple handling of the Application

It shall be easy to start and play the application. It shall be easy to learn and handle the 
control of the application itself. The user interface shall be simple and intuitive. 

### 3.2.2 Usability Requirement Two - Simple handling of the Main Character

It shall be easy to control the main character, on the computer as well as on the smartphone.
The control shall be intuitive and simple.

### 3.2.3 Usability Requirement Three - Application Crash

When the application crashes for minor reasons that do not affect the user, the user 
shall not get to know it. The application shall rebuild itself.

### 3.2.4 Usability Requirement Four - Tutorial

There shall be a tutorial in the beginning of the game after the first start. It shall be 
possible to always access the tutorial.
This requirement is outdated for the actual scope.

### 3.2.5 Usability Requirement Five - Report to the Developers

The user shall have a way to report a problem or give positive and negative feedback.
This requirement is outdated for the actual scope.

### 3.2.6 Usability Requirement Six - Leave Game 

It shall be possible to leave the game at any time. By pressing "escape" on the keyboard, there shall be shown a sub menu if the user 
want to either resume or leave the game.
Also when leaving the game by clicking on "X" on the top of the window, the application shall stop.

## 3.3 Reliability

### 3.3.1 Reliability Requirement One - Fluent Gameplay

While using the application, it shall be fluent. There shall no stuttering or long pauses.

### 3.3.2 Reliability Requirement Two - Application Crash

When the application crashes, Unity provides an crash handler itself.

## 3.4 Performance

### 3.4.1 Performance Requirement One - Performance

The application shall run at atleast 30 FPS.

### 3.4.2 Performance Requirement Two - User Capacity

The game shall be for a single user only as per installation.

### 3.4.3 Performance Requirement Three - Local Resources

The application shall run at a minimum disk space and shall run independendly from the 
operating system. It application shall also not use too much memory space.

## 3.5 Supportability

### 3.5.1 Supportability Requirement One - Maintainable Code

The source code shall be kept simple and so, it shall be easy to maintain. The code shall 
be divided into a MVC-relied way.

### 3.5.2 Supportability Requirement Two - Reported Bugs

Reported bugs shall be updated in the source code every month. So, many bugs can be fixed in 
one time and the time to maintain the code is reduced.
This requirement is outdated for the actual scope.

## 3.6 Design Constraints

### 3.6.1 Design Constraint One - Architecture

Since the architecture is to be MVC, the source code is divided in three separate parts.

### 3.6.2 Design Constraint Two - Models

Since the team only uses open-source tools, the team is kept low with every tool. Otherwise
there shall be used way more tools.

### 3.6.3 Design Constraint Three - Development Tools

We decided to use the following tools, to help developing the game:</br>

<ul>
<li><b>YouTrack</b> Project Management and Issue Tracker Sytem</br></li>
<li><b>GitHub</b> Version Control System</br></li>
<li><b>Unity</b> Game Engine</br></li>
<li><b>Visual Studio</b> IDE used for scripting within Unity</br></li>
</ul>

## 3.7 Online User Documentation and Help System Requirements

There shall be a link to report bugs in the settings of the application. 
This requirement is outdated for the actual scope, since the internet connection is not required yet.

## 3.8 Purchased Components

Ted's Entertainment has not bought anything in order to develop the game.

## 3.9 Interfaces

The application shall be runt on smartphones and computers. 
The used interface is decided by the Unity Framwork.

### 3.9.1 User Interfaces

There shall be a dark mode and a light mode, chosen by the user. Initially the light mode is 
turned on.
This requirement is outdated for the actual scope.

### 3.9.2 Hardware Interfaces

The application is mostly hardware indepenent. At the time of the first official release, 
the application is available for both operating systems, Windows and Mac OS. In a further release, 
the application shall be available for Android-based smartphones.

### 3.9.3 Software Interfaces

There are no software interfaces implemented since all connections go to and come from the Unity Framework.

### 3.9.4 Communications Interfaces

Refer to above 3.9.3.

## 3.10 Licensing Requirements

The application shall be open source under the GPL version 2 or any later version.

## 3.11 Legal, Copyright, and Other Notices

The developers are not responsible for any impact, the game might have on the user.

## 3.12 Applicable Standards

There are no used standards that can be referenced to.

# 4. Supporting Information

The application contains a link to the GitHub repository. There, all necessary documents can be found.
