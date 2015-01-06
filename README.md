##Postman Collection for Tableau's REST API
================

This is a .json file for importing into [Postman](http://www.getpostman.com/), a tool for making HTTP requests via the browser.

To import, open Postman, click on the Collections tab in the upper-left hand corner and click the Import Collection icon.

### What's in this collection
Essentially it has all of the requests that the REST API can currently make. This is the same list as found in the [Rest API Documentation](http://onlinehelp.tableausoftware.com/v9.0/server/en-us/help.htm#rest_api_ref.htm#API_Reference%3FTocPath%3DREST%2520API%7CAPI%2520Reference%7C_____0).

### So how do you use this?
The documentation is your friend. This collection is not a replacement for that, but a convenience for testing out what you learn in the documentation. In addition, there is an [online video to assist you in getting started with the REST API.](http://www.tableausoftware.com/learn/tutorials/on-demand/rest-api)

Most calls require IDs for objects. For instance if you want to find out what workbooks were published by a specific user on a specific site, you will need to query the site to find it's id and then you will need to query the users on that site to find the id of the specific user.

All of these functions are present in this collection, but you must replace the authToken and IDs that appear and also the server url/ip to point it at your installation of Tableau Server.

For more information see the file titled API Reference.pdf

### Updated for 9.0
9.0 added many useful functions to the REST API including Project management, Group management, Permissions management, downloading, publishing, and more. This collection has been updated to reflect those changes.
Note: The functions for publishing are in this collection, but POSTman will set the content-type to multipart/form-data, while the api is expecting multipart/mixed. So for using POSTman to test publishing, you can make the request from POSTman, it will fail, but then you can open the request in an application like Charles or Fiddler, modify the request to change it to multipart/mixed and it should work.

###Warning
This collection is not officially 'blessed' by Tableau Engineering or Support.
What does that mean? We didn't have a qa team test it. It's a tool for learning how to use the REST API and shouldn't be used for more than that.
You should not expect that there are 0 bugs.

If you have problems getting it to work, feel free to Email us with questions, but we won't promise quick responses.

Sorry =)