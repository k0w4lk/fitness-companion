# Authentication

## US-1: As a user, I want to register in app via email to access relevant functionality

### Features:  

- #### Email + password registration:  
    **AC**  
    1. [FE] On client startup if there is no stored user data register page is loaded (/auth/register)
    2. [FE] By default there is register form with following units:
       - title (L-1)
       - first name input
       - last name input
       - email input
       - password input
       - password confirm input
       - Client/Trainer radio buttons  
       - Submit button
       - link to login page
    3. [FE] By clicking on *Submit button* app sends [POST register request](/docs/technical/auth-api.md).
    4. [BE] on recieving register request server validates payload and creates user into users table
    5. On success user need to be redirected to his profile page. On error there is alert with error message.

### I18n
 ||RU|
 |-|--|
 |1|Регистрация|
