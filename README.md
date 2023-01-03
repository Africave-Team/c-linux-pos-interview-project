# C/C++ Developer/Linux POS Software Engineer Interview Project

These are small projects for a Linux POS Software Engineer to be interviewed at Africave

## Project 1 - Basic Communication App
Build a C app that consume an API endpoint for authentication, access a protected API endpoint by sending an authorization token as bearer in the header and display the response in a user-friendly way to the best of your knowledge. Finally, add an FTP client that will download a file from the server to the app. From the file downloaded, display the file name, file type and file size.

#### Resources
1. Authentication endpoint: http://linuxpos.byethost4.com/api/login
    ```
    POST {"username": "testuser", "password":"test123@$2023"} 
    HEADER ContentType: application/json, Accept: application/json
    ```
2. Protected endpoint: http://linuxpos.byethost4.com/api/services
    ```
    GET
    HEADER ContentType: application/json, Accept: application/json, Authorization: Bearer token
    ```
3. FTP Details
    ```
    host:ftp.byethost4.com
    port:21
    username:b4_33308266
    password:l1nuxp052023
    path:/htdocs/resources
    ```

## Project 2 - EMV Implementation
Buid an application that reads all card (EMV process) e.g MasterCard, Verve, Visa and generate ISO 8583 messages that is ready for **NIBSS** submission for the following transactions:
 - Preauth
 - Preauth Completion
 - Purchase
 - Purchase with cashback
 - Reversal
 - Balance Enquiry

The application is expected to work on any of the following Linux POSs: NEWPOS/SZFP 8210, 7210, Newland ME31.

You are expected to use DUKPT encryption for the Track2 and Pinblock with the following credentials:
```
BDK: 0123456789ABCDEFFEDCBA9876543210
KSN: FFFF9876543210E00000
```

How the user interface should look like depends on you. 

#### Good Luck