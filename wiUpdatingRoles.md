# Updating Puppet Roles

# Table of Contents
  
- [Changelog](#Changelog)
- [Introduction](#Introduction)
- [Purpose](#Purpose)
- [Scope](#Scope)
- [Stages For AddingRoles](#Stages-For-Adding-Roles)
- [Updating Roles Procedure In VRA Resources](#Updating-Roles-Procedure-In-VRA-Resources)
- [Updating Roles Procedure In VRO Resources](#Updating-Roles-Procedure-In-VRO-Resources)


# Changelog
  
| Version | Date       | Description      | Author       |
| ------- | ---------- | ---------------- | -------------|
| 0.1     | 21/09/2022 | Updating Puppet Roles In ANS-MAR, CLY  | Vadlamudi Manjusha |

# Introduction

## Purpose

The purpose of this document is to create step by step instructions for adding and updating puppet roles whenever new requests comes from client side.

## Scope

The scope of this document covers the following:

     Adding Puppet Role/Tag in ANS-MAR, ANS-CLY Environment

# Stages For Adding Roles

      If we get any requests to add or update puppet role , There are two places where we have to make changes

              1. The first one is in Blueprint.
              2. The second one is in vro workflow which is present under Resources.
	      
## Prerequisites

     -  Access to the both ANS-MAR , CLY in VRA Environment
     -  Access to the both ANS-MAR , CLY in VRO Environment

## Stage 1
	      
## Updating Roles Procedure In VRA Resources

- Stage 1.1
       
       -  For updating roles in Blueprint , Log on to the VRA Service Broker
 
 ![Figure 1](images/Picture1.png)
  
- Stage 1.2  
     -  For mapping the roles select content&policies tab.
     -  Click on content&policies select content and then select the blueprint which we want to edit.
     -  Click on the option there we can see the customize form.
   
 ![Figure 1](images/Picture2.png)
 
- Stage 1.3
     -  In customize form , Here we can see the role properties.
     -  Under the role properties we can find the values option where we can edit the values.
     
 ![Figure 1](images/Picture3.png)
 
- Stage 1.4
     -  Whenever we have to update roles, It should be always in Lexographical order.
     -  Whatever roles we have to update it in the form of key-value pair.
## For Example:
     enreg::service_batch::init:|ENREG SERVICE BATCH
 
- Stage 1.5 
     -  After updating roles, We can verify it under catalog.
     
 ![Figure 1](images/Picture4.png)   
 
- Stage 1.6 
     - In request form , we can see that values are updated.
     - Those roles can be used for provisioning.
     
 ![Figure 1](images/Picture5.png)
    


## Stage 2

## Updating Roles Procedure In VRO Resources

- Stage 2.1
   
     - The purpose of updating tags in vro that tag should be available under day2 action such as "update puppet tag"


![Figure 1](images/Picture6.png)
  
- Stage 2.2  
     - Click on the Resources which is present under the Assests tab.
     
![Figure 1](images/Picture7.png)
 
- Stage 2.3 
     - under resource folder we will find "role.txt".
     - We should export this file and add/edit the tag by following key|value format and then upload the same by cliking on update option as given in screenshot.
     - After importing the file click on Save.
     
## Note :  
     - Keep the file name same , If we change the file name the code will gets changed.
     
     
![Figure 1](images/Picture8.png)     
     

## Note :

    - Same steps will be followed for ANS-CLY Environment.
    - Same steps will be applied for both DEV and PRD Blueprints.
    







