# Pen Testing Live Targets

Time spent: **2** hours spent in total

> Objective: Identify vulnerabilities in three different versions of the Globitek website: blue, green, and red.

The six possible exploits are:

* Username Enumeration
* Insecure Direct Object Reference (IDOR)
* SQL Injection (SQLi)
* Cross-Site Scripting (XSS)
* Cross-Site Request Forgery (CSRF)
* Session Hijacking/Fixation

Each color is vulnerable to only 2 of the 6 possible exploits. First discover which color has the specific vulnerability, then write a short description of how to exploit it, and finally demonstrate it using screenshots compiled into a GIF.

## Blue

Vulnerability: Session Hijacking

Description: Using the session id manipulation link provided by codepath. I was able to login into the same account by changing the session id to an account that was already loggged in.

GIF Walkthrough: <img src='https://github.com/Ybrahm22/Pen-Testing-Live-Targets/blob/main/Blue_SessionHijacking.gif' title='Session Hijack' width='' alt='Session Hijack' />


## Green

Vulnerability: User Enumeration

Description: On the site login page, if a user attempts to login with a username present in the database but with an incorrect password an error prompt will show up in all bolded characters. However, if a login is attempted with a username that is not present in the database, the error prompt will show up unbolded. 

GIF Walkthrough: <img src='https://github.com/Ybrahm22/Pen-Testing-Live-Targets/blob/main/Green_UserEnumeration.gif' title='User Enumeration' width='' alt='User Enumeration' />



## Red

Vulnerability: IDOR

Description: Upon manipulating the URL we are able to land onto a page that we should not be able to see

GIF Walkthrough: <img src='https://github.com/Ybrahm22/Pen-Testing-Live-Targets/blob/main/Red_Idor.gif' title='IDOR' width='' alt='IDOR' />






