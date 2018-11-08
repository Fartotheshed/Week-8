# # Project 8 - Pentesting Live Targets

Time spent: 4 hours spent in total

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

Vulnerability #1:SQL Injection
GIF Walkthrough:
![blue1](https://user-images.githubusercontent.com/23129522/48169142-04631280-e2c0-11e8-8c31-370c6cbb1575.gif)
Typed in some SQl in the url for each site, but in the blue site it shows that the database fails.

Vulnerability #2:Session Hijacking/Fixation
GIF Walkthrough:
![blue2](https://user-images.githubusercontent.com/23129522/48169210-5c017e00-e2c0-11e8-9241-af1393962b22.gif)
Used a different browser and changed the session id. I was able to log in with the bue site but not the green and red.

## Green

Vulnerability #1:Cross-Site Scripting
GIF Walkthrough:
![green1](https://user-images.githubusercontent.com/23129522/48169314-c9adaa00-e2c0-11e8-8bb3-c22a8999c426.gif)
Typed in some javascript where we could post feedbacks. In the green site it shows the vulnerability.

Vulnerability #2:User Enumeration
GIF Walkthrough:
![green2](https://user-images.githubusercontent.com/23129522/48169370-0d081880-e2c1-11e8-85df-fae436eb1c76.gif)
Used different logins. If the login existed, the 'Login Unsuccessful' would be bold. If the the login did not exist, it would not be bold.

## Red

Vulnerability #1:Insecure Direct Object Referencing
GIF Walkthrough:
![red1](https://user-images.githubusercontent.com/23129522/48169569-bd761c80-e2c1-11e8-8d53-94a6b651201a.gif)
Changed the id of each url for each site. In the red site the vulnerability shows if the id is greater than 9.

Vulnerability #2:Cross-Site Request Forgery
GIF Walkthrough:
![red2](https://user-images.githubusercontent.com/23129522/48169668-28bfee80-e2c2-11e8-89d7-97f681568a91.gif)
Inspected the element for each site of the users. Changed the token of each site. Info of the user would show only for the red site after the token was changed.

## Notes

One trouble I had was knowing where to write the code.

