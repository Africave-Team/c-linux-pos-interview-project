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
