The robot performs the following steps:
1- Read the config.csv file 

2- Wait until you receive the test email on your email inbox then read it and download the attached
excel file:
- The email subject: maids.cc RPA test
- The attached excel file name: ‘test.xlsx’ example
- Add the downloaded file to the output folder

3- Go to https://hide.me/en/ website and create an account (even if you already have an account,
go to the sign-up page) then insert your email and click on register:

      a- If you don’t have an account, you will receive an activation email, activate it and create an account (insert username and password) then logout and login again 

      b- if you already have an account, you will receive an email asking you to change your password, open the change password link then change it, the website will navigate you to the home page, you should logout and login (using username and password) again

4- Open the hide.me VPN desktop application and enable VPN (don’t need to add an account)

5- Read the data table from the download excel file

6- Foreach record in the data table, do the following steps:

      a. Go to https://www.fakenamegenerator.com/ and select gender and country and click on
generate button then get the info:
Name
Password
Birthday
Address
Phone
Country code
Company
Occupation

      b. Save the extracted data in the result excel file (mentioned in step 6.e)

      c. Go to https://automationexercise.com/ and click on sign up then insert the username
and email and fill the user information and click on create account (make sure that the account has been created) then click on continue and delete it

      d. Call this API: https://reqres.in/api/users to add the user info then get the id from the
response:
            i. End point: https://reqres.in/api/users
            ii. Method: POST
            iii. Body:
            {

            "name": "Ronald Beaman",
            "birthday": "1980-12-11 ",
            "address": "311 Burning Memory Lane",
            "phone": "215-289-4533",
            "countryCode": "1",
            "company": "Red Robin Stores",
            "occupation": "Dredge operator"
            }
            
      e. Save data in the following files:
            o result.xlsx: contains the user extracted date in step 7.b example
            o summary.csv: contains the transactions result example:
Start Date: start date of the transaction
End Date: end date of the transaction
User ID: the id value that we get it in step 7.d
Username: the username that we get it in step 7.a
Status: Completed / Failed
Error Message: the error message if the status is failed and empty it it’s completed
Screenshot Path: screenshot of the error
7- Send the result.xlsx and summary.csv files via email to receiver emails

8- Wait until you receive a new email, if you didn’t receive an email for 5 mins then stop the
process.
