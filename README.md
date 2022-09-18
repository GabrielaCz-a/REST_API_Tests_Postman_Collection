# REST_API_Tests_Postman_Collection
## ABOUT PROJECT
This is my sample test cases collection for testing REST API created in Postman.

Documentation for tested REST API: [https://thetestingworldapi.com/Help](https://thetestingworldapi.com/Help)

The collection contains positive and negative test cases with collection variables and assertions.
Not every test case will have a positive result.
Here you have the list of fail TC's with my comment:
* "**Add_Student_Without_Body**" - in this case you try to create a new student without any data in body with POST method. This API allow you to do this and response from the server is "201 Created". However it is consistent with the documentation, in my opinion in this case API should return "400 Bad request".
* "**Add_Student_Adress_Without_Id**"- in this case you try to add address without student id (in other words, add the data without specifying the resource they relate to).
This API allow you to do this and response from the server is 200 OK. However it is consistent with the documentation, in my opinion in this case API should return "400 Bad request" and student id should be required.

## HOW TO RUN
To see the collection you have to download JSON file "REST API-Testing World (Student Data)" and next import this file in Postman.
You can run automatically the whole collection, you can run automatically folders and you can also send request by request, manually. After executing test cases you will see the test result for every request.
