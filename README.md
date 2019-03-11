# OracleAPEX-forgot-password
Oracle APEX forgot password method for APEX authentication for end users. Yes, a working method for change password not-authenticated user. But with a not-safe procedure. This is just core-method. Not working on apex.oracle.com!

# DEMO

https://apex.oracle.com/pls/apex/f?p=15184
* Any given e-mail address will receive a verification code

![1](https://user-images.githubusercontent.com/26149665/54110115-96576500-43f1-11e9-8bed-656c10c25433.jpg)

# Requirements

- Any Apex Application with application express authentication (NOT custom authentication. Also not working on apex.oracle.com right now)

# Key for change password for not-authenticated user: CALL PASSWORD CHANGE PROCEDURE AS SCHEDULED JOB 

As you know, you have to be authenticated to call apex api functions. But you can run api functions as scheduled job. 

- Create a stored procedure to change the passwords
- Create a Scheduled Job to call stored procedure
