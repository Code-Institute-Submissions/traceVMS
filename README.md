<div align="center">
<img src="https://github.com/tdignan87/traceVMS/blob/master/static/img/TSLogo.jpg" target="_blank" rel=""/>
</div>
<div align="center">
<h1>TraceVMS Visitor & Contractor Management System</h1>
</div>

## Introduction

TraceVMS was created by myself as I noticed through my day job that most factories and food companies use paper based systems for recording visitors to the site.
I can see the headache of paper based systems from working in the manufacturing industry for over 10 years. TraceVMS hopes to help with that problem by recording visitor and contractor information to help with record keeping, reduce paperwork and adhere to food safety compliance(BRC).

Tracesense is my own company i created in November 2019 and decided to go with that name for the software.

## Table of Contents
1. [UX](#example)
    - [Project Goals](#example2)
    - [User Goals](#third-example)
    - [Business Goals](#fourth-examplehttpwwwfourthexamplecom)
    - [Developer Goals](#fourth-examplehttpwwwfourthexamplecom)
    - [User Requirements & Expectations](#user-stories)
        - [Design Choices](#user-stories)
    - [WireFrames](#wireframes)
    - [Flow Chart](#flow)
    

2. [Features](#example)
    - [Existing Features](#background)
        - [Register Visitor Page](#background)
        - [Admin Page](#background)
        - [About Page](#background)
        - [Administrator Login Page](#background)
    - [Features Deployed](#background)
    - [Features Left To Implement](#background)


3. [Information Architecture](#information-architecture)
    - [Database choice](#database-choice)
    - [Data Storage Types](#data-storage-types)
    - [Collections Data Structure](#collections-data-structure)
        - [Users Collection](#users-collection)
        - [Activities Collection](#activities-collection)

4. [Technologies Used](#technologies-used)

5. [Testing](#testing)

6. [Deployment]
    - [Heroku Deployment](#background)
    - [How to run this project locally](#background)

7. [Credits]
    - [Content]
    - [Media]
    - [Code]
    - [Acknowledgements]

8. [Contact]

9. [Disclamer]
  

----

# UX

## Project Goals

The goal of this project is to create a suitable, easy to use application for recording visitors and contractors to your site. The software is aimed at food manufacturers specifically designed to help them be compliant with contractor management and also health and safety requirements. The system's focus will be ease of use for data input and data retrieve.

## User Goals
User goals are:

- Have a system for recording visitors to my site so i can remove paperwork records.

- Have confidence in the system so it keeps us compliant with food safety requirements.

- Ease of use and can be used across any device.

- Secure so data is compliant with GDPR.

- Functionality to add new questions to ask visitors and contractors as legislation changes.

## Business Goals

The target businesses to use this application are:

- Bakeries
- Food & drink manufacturers

Business user goals are:

- A well thought out, designed, user friendly platform that will benefit customers who need compliance.

- A user interface that allows me to input the data efficiently.

- Value for money (site is for a project, but eventually i will use this as part of my new business). I want the software to exceed requirements for the user as word of mouth spreads fast
in the food industry in scotland.

## Developer Goals

Developer goals are:

- Provide an effective, easy to use site for customers to add new visitors to there premises, ensure they have completed the compliance checks and data stored in the database correctly.

- I can learn more about frontend and backend technologies together for the first time.

- This is currently a student project although the future goal of traceVMS is to eventually sell it to manufacturers to use on there sites. This will come later when my experience in development gets better.

## User Requirements & Expectations

### Customer Stories

As a customer to traceVMS i expect/want/need:

1. To easily navigate across the application, the layout needs to make sense so i'm not put off from using the system and just stick to paper.

2. The information presented needs to be in a practical way for me to digest and follow easily. I need to be able to use the app quickly and efficiently as contractors may not have a lot of time at the customers site.

3. I need to have sufficient confidence in the system so i can remove paperwork from my processes. The system needs to tick the box for storing the data, and for us to retrieve it if we get audited from the BRC or Health and Safety executive. 

4.To use the administrator set up panel to be able to filter out on who is approved, not approved contractor and any other key information required.

5.I want to be able to search for users who have completed the site induction.

6. I want to be able to search for a list of everyone who is currently on site in case this needs to be printed in used in a fire evacuation emergency. I need to be able to print the list from the browser of the names of people on site. 

7. I want to be able to access data easily and within the 4 hour maximum BRC timeframe for retrieving company audit data.

### Developer Stories

As the developer and owner of traceVMS i expect/want:

1. To be able to create, delete, update, and read information to the database.

2. Allow customers to find the application easy to use.

3. The software helps and improves compliance.

4. For secure login to the administrator panel to amend the lists.

5. The data is secure and complies with GDPR for the customer.

6. The system is reliable for use and gives confidence the customer can remove the paperwork.


## Design Choices

traceVMS application has a professional feel that doesnt look too over complicated for the user. The following design choices were made:

### Fonts

* The google font applied across the whole application was 'lato' with a fall back of sans-serif. Lato feels very modest and text sizes look great either large or small. The font is easily recognizable.


### Colours

* The colors for this project were choosen based on the two primary colours in my company logo. These colours are

1. Dark Blue: CMYK 100,50,10,0; RGB 0,105,68; HEX #0069A8
2.Light Blue: CMYK 65,0,10,0; RGB 66,191,224; HEX #42BFE0

The Dark Blue #0069A8 was used for button controls and blended well with etiher the lighter blue background or the white background depending where it was placed. The light blue was my jumbotron's background colior and background colour for the menu choices option. 

I feel the colours i have chosen have complimented eachother well and blend well with the company logo.

## Wireframes

These wireframes were created using [Balsamiq](https://balsamiq.com/) during the scope part of the design and planning process for this project. I found Balsamiq very useful for helping me plan out exactly what i needed for my application to come together.

Links to be updated
- [Browser Home Page](https://ibb.co/52Z3P4r)
- [Browser Visitor Sign In Page](https://ibb.co/Wcgbtqs)
- [Browser Visitor Sign Out Page](https://ibb.co/Nm8FYbd)
- [Browser Administrator Set Up Page](https://github.com/tdignan87/traceVMS/blob/master/Wireframes/Browser%20Administrator%20Set%20Up.png)
- [Browser Add New Company Page](https://github.com/tdignan87/traceVMS/blob/master/Wireframes/Browser%20Add%20New%20Company.png)
- [Browser Edit Company Page](https://ibb.co/njnP5C5)
- [Browser Delete Company Page](https://ibb.co/1TyV9sN)
- [Browser Add Questions Page](https://github.com/tdignan87/traceVMS/blob/master/Wireframes/Browser%20Add%20New%20Question.png)
- [Browser Edit Questions Page](https://ibb.co/nr2s9cw)
- [Browser Delete Questions Page](https://github.com/tdignan87/traceVMS/blob/master/Wireframes/Browser%20Delete%20Questions.png)
- [Mobile Home Page](https://ibb.co/sqj60xb)
- [Mobile Visitor Sign In Page](https://ibb.co/sqj60xb)
- [Mobile Visitor Sign Out Page](https://ibb.co/sqj60xb)
- [Mobile Admin Set Up Page](https://ibb.co/sqj60xb)
- [Mobile Visitor Edit Page](https://ibb.co/sqj60xb)
- [Mobile Visitor Delete Page](https://ibb.co/sqj60xb)
- [Mobile Company Add New](https://ibb.co/sqj60xb)
- [Mobile Company Edit](https://ibb.co/sqj60xb)
- [Mobile Company Delete](https://ibb.co/sqj60xb)
- [Mobile Questions Add New](https://ibb.co/sqj60xb)
- [Mobile Questions Edit](https://ibb.co/sqj60xb)
- [Mobile Questions Delete](https://ibb.co/sqj60xb)
- [Tablet Home Page](https://ibb.co/sqj60xb)
- [Tablet Visitor Sign In Page](https://ibb.co/sqj60xb)
- [Tablet Visitor Sign Out Page](https://ibb.co/sqj60xb)
- [Tablet Administrator Page](https://ibb.co/sqj60xb)
- [Tablet Add New Company Page](https://ibb.co/sqj60xb)
- [Tablet Edit Company Page](https://ibb.co/sqj60xb)
- [Tablet Delete Company Page](https://ibb.co/sqj60xb)
- [Tablet Add New Visitor Page](https://ibb.co/sqj60xb)
- [Tablet Edit Visitor Page](https://ibb.co/sqj60xb)
- [Tablet Delete Page](https://ibb.co/sqj60xb)

## Flow Chart

This flowchart was created on Microsoft Powerpoint to explain the flow of how the application should run.
User flowchart:
<img src="https://github.com/tdignan87/traceVMS/blob/master/Wireframes/flowchart/flowchart-one.jpg" target="_blank" rel=""/>


Administrator options:
<img src="https://github.com/tdignan87/traceVMS/blob/master/Wireframes/flowchart/admin_options.jpg" target="_blank" rel=""/>

## Features

## Information Architecture

### Database Choice

A SQL database structure i think would have been more suitable for this project however the requirements were to use mongoDB. I have experience with Firebird, and SQL server already so i'm looking forward to learning more about MongoDB and gain some experience with it.

To have easy access to relational data, inner objects were used inside the data structure so that they could be accessed and looped through for combo boxes and where else required.

### Data Storage Types

The types of data stored in MongoDB for this project are:
- ObjectId
- String
- Boolean
- DateTime


### Collections Data Structure

TraceVMS relies on the following structure

#### Administrator login

| Title | Key in db | form validation type | Data type |
--- | --- | --- | --- 
admin_id | _id | None | ObjectId 
Name | username | text | string
Password | password | text | string
role | role | text | string

#### Visitors On Site

|Title | Key in db| form validation type| data type |
--- | --- | --- | ---
visitorsID | _id | none | ObjectId
Name | name | text| string
Company | company | text | string
Visiting | visiting | text |string
entered_bakery| entered_Bakery| boolean | bool
sign_in_timestamp|sign_in_timestamp| timestamp |timestamp

#### Contractors

|Title| Key in db | form validation type | data type |
--- | --- | --- | ---
contractorID | _id | none | ObjectId
Name| Name| text|string 
Address | Address| text | string
Approved| isApproved| checkbox | boolean

#### Questions

|Title| Key in db| form validation type| data type |
--- | --- | --- | ---
questionID | _id| none | Objectid
Question| question | text | string
Answer_First | Answer_First| text | string
Answer_Second | Answer_Second| text | string
