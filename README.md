Install Nodejs (https://nodejs.org/dist/v8.10.0/node-v8.10.0-x64.msi) 


Install ExpressJS (https://expressjs.com/en/starter/installing.html)


Create AWS account for aws s3 service (https://portal.aws.amazon.com/billing/signup#/)


Change the CORS policy as following ( go to Console → Amazon S3 → your_bucket → Permissions→ CORS configuration)

<?xml version="1.0" encoding="UTF-8"?>
<CORSConfiguration xmlns="http://s3.amazonaws.com/doc/2006-03-01/">
<CORSRule>
    <AllowedOrigin>http://localhost:8000</AllowedOrigin>
    <AllowedMethod>PUT</AllowedMethod>
    <MaxAgeSeconds>3000</MaxAgeSeconds>
    <ExposeHeader>x-amz-server-side-encryption</ExposeHeader>
    <ExposeHeader>x-amz-request
-id</ExposeHeader>
    <ExposeHeader>x-amz-id-2</ExposeHeader>
    <AllowedHeader>*</AllowedHeader>
</CORSRule>
</CORSConfiguration>


Change the directory to file cc.js and then Run cc.js file from the folder


Goto folder and open the frontend.html page


To upload the video copy the file path and paste it enter file path textfield and give a unique name to the video and click to upload


For the usage of the service go to Console → Amazon S3 → your_bucket → Management → Metrics
