# WordpressvsKali
# Project 7 - WordPress Pen Testing

Time spent: **9** hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pen Testing Report

### 1. (Required) Vulnerability Name: Username enumararion

- [ ] Summary: Find valid usernames using wpscan
   
- [ ] GIF Walkthrough: 
    <img src="https://github.com/Tanya703/WordpressvsKali/blob/f9a78275c7e7b49ab38b30d820448d43e6120e7f/usernames.gif" width="800">
- [ ] Steps to recreate: 

      wpscan --url http://127.0.0.1:8080 --api-token YOUR_TOKEN -e u vp 

  

    
### 2. (Required) Vulnerability Name: Password Enumeration

- [ ] Summary: Find correct passwords for the usernames found in previous challenge using wpscan
  
- [ ] GIF Walkthrough: 
<img src="https://github.com/Tanya703/WordpressvsKali/blob/6b33a6bd14b4ebfd52dbbeb7e084660c38448710/6yrqgi.gif" width="800">
- [ ] Steps to recreate: 
wpscan --url http://127.0.0.1:8080 --api-token YOUR_TOKEN --usernames username.txt --passwords password.txt

username.txt → a file with usernames found from Username enumeration scan. 

password.txt → a file with known passwords, use a sample size. 

    

### 3. (Required) Vulnerability Name: Unauthenticated Stored Cross-Site Scripting

- [ ] Summary: Insert a script that goes to a codepath website in comment section of the website.
  
- [ ] GIF Walkthrough: 
 <img src="https://github.com/Tanya703/WordpressvsKali/blob/6b33a6bd14b4ebfd52dbbeb7e084660c38448710/Cross-SiteScripting.gif" width="800">
- [ ] Steps to recreate: 

insert "<body onload=window.location='https://codepath.org/'>" in comment section


    
