# QA_API_Testing


# Api_Testing_Assessment
**GoREST API Testing with Postman**

This project contains a Postman Collection and Environment for testing CRUD operations on the GoREST public API
.

**Files Included**

Gorest.postman_collection.json
Postman Collection containing all API requests (View, Create, Patch, Update, Delete).

Gorest.postman_environment.json
Postman Environment file with required variables like base_url and authToken.

**Setup Instructions**
1. Install Postman

Download & install from: https://www.postman.com/downloads/

2. Import Collection & Environment

Open Postman

Click Import → File

Import both files:

**Gorest.postman_collection.json**

**Gorest.postman_environment.json**

   **Select Environment**
After importing, select Gorest Environment from the top-right in Postman.

This environment already contains:

base_url = https://gorest.co.in

authToken =<token>

 No manual editing is required unless you want to update the token later.

**How to Execute the Tests**

Select the environment “GoREST Environment” from the dropdown (top-right).

Open the “Gorest” collection.

You can either:

Run requests individually by clicking on each request.

OR click on the collection → Run Collection to execute all tests at once.

(Set delay = 2 seconds between requests for smooth execution.)

 **Test Execution Summary**

**1.View User**

Method: GET

Expected Status Code: 200 OK

Actual Status Code: 200 OK

Result:  Pass

**2.Create User**

Method: POST

Expected Status Code: 201 Created

Actual Status Code: 201 Created

Result:  Pass

**3.Status Verification**

Method: POST

Expected Status Code: 422 Unprocessable Entity

Actual Status Code: 422 Unprocessable Entity

Result: Fail (status is not valid)

**4.Patch User**

Method: PATCH

Expected Status Code: 200 OK

Actual Status Code: 200 OK

Result:  Pass

**5.Update User**

Method: PUT

Expected Status Code: 200 OK

Actual Status Code: 200 OK

Result: Pass

**6.Delete User**

Method: DELETE

Expected Status Code: 204 No Content

Actual Status Code: 204 No Content

Result:  Pass
