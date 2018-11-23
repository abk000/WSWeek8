# Project 8 - Pentesting Live Targets

Time spent: **3** hours spent in total

> Objective: Identify vulnerabilities in three different versions of the Globitek website: blue, green, and red.

The six possible exploits are:
* Username Enumeration
* Insecure Direct Object Reference (IDOR)
* SQL Injection (SQLi)
* Cross-Site Scripting (XSS)
* Cross-Site Request Forgery (CSRF)
* Session Hijacking/Fixation

Each version of the site has been given two of the six vulnerabilities. (In other words, all six of the exploits should be assignable to one of the sites.)

## Blue

Vulnerability #1: SQL Injection

<img src="https://i.imgur.com/eiyLYIs.gif"/>

The injection shown causes a forced delay in page loading. 

Vulnerability #2: Session Hijack

<img src="https://i.imgur.com/uhxeklc.gif" />

I was able to use the php session id for a logged in session in one browser, to log in without a password in another. 

## Green

Vulnerability #1: Username Enumeration

<img src="https://i.imgur.com/JPqXqRH.gif"/>

The mistake the developer made here was bolding the error message for existing usernames but not for others. 

Vulnerability #2: Cross-Site Scripting

<img src="https://i.imgur.com/qHVjkGW.gif"/>

A XSS vulnerability in the contact form. Since other students performed the attack as well, several pop-ups are shown. 

## Red

Vulnerability #1: Insecure Direct Object Reference 

<img src="https://i.imgur.com/SktXoZ3.gif"/>

Vulnerability #2: Cross Site Request Forgery

<img src="https://i.imgur.com/K38GaMV.gif"/>

Using the feedback form, have an admin follow a given link to an html site that will take advantage of the admin session to update 
info on the employee. 

## Notes

Describe any challenges encountered while doing the work
