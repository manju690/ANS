# Updating Puppet Roles

# Table of Contents
  
- [Changelog](#Changelog)
- [Introduction](#Introduction)
- [Purpose](#Purpose)
- [Scope](#Scope)
- [AddingRoles](#AddingRoles)
- [Updating Roles Procedure In ANS-MAR Under VRA Environment](#Updating-Roles-Procedure-In-ANS-MAR-Under-VRA-Environment)
- [Updating Roles Procedure In ANS-MAR Under VRO Environment](#Updating-Roles-Procedure-In-ANS-MAR-Under-VRO-Environment)


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
	      
## Updating Roles Procedure In ANS-MAR Under VRA Environment

## Stage 1.1
     -  For updating roles in Blueprint , Log on to the VRA Service Broker
 
 ![Figure 1](Picture1.png)
  
## Stage 1.2  
     -  For mapping the roles we can see under the design part in content&policies.
     -  Click on content&policies under that content and then to respected blueprint.
     -  Click on to the customize form.
   
 ![Figure 1](Picture2.png)
 
## Stage 1.3
     -  In customize form , here we can see the role tab.
     -  When we click on that role tab , on the right hand side we can see the constant which is present under values.
     -  Copy the constant value and paste it in the notepad.
   
 ![Figure 1](Picture3.png)
 
## Stage 1.4
     -  Whenever we have to update roles, It should be always in Lexographical order.
     -  Whatever roles we have to update it in the form of key-value pair.
     -  When we have to add new role , Just click on comma( , ) and provide the value of that particular role and then key.
     
 ![Figure 1](Picture4.png)  
 
## Stage 1.5 
     -  When roles have been updated successfully, We can verify it under catalog.
     
 ![Figure 1](Picture5.png)   
 
## Stage 1.6 
     - In request form , we can see the key-value pairs of that role.
     - Click on Submit.
     - Those roles should be updated by provisioning.
     
 ![Figure 1](Picture6.png)
    


## Stage 2

## Updating Roles Procedure In ANS-MAR Under VRO Environment

## Stage 2.1
    - To update those roles actually as a part of day-2-action , We have to add that roles under VRO.
   
 ![Figure 1](Picture7.png)
  
## Stage 2.2  
     - Click on the Resources which is present under the Assests tab.
     
 ![Figure 1](Picture8.png)
 
## Stage 2.3 
     - Click on  export the file and do the changes and then Import the file.
     - Keep the file name same , If we change the file name the code will get changed.
     - After importing the file click on Save.
     
 ![Figure 1](Picture9.png)




## Note :

    - The above procedure in ANS-MAR is applied for dev
    - Same procedure will be done for both PRD And DEV in ANS-CLY Environment







