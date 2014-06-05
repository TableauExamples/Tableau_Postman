##Postman Collection for Tableau's REST API
================

This is a .json file for importing into [Postman](http://www.getpostman.com/), a tool for making HTTP requests via the browser.

To import, open Postman, click on the Collections tab in the upper-left hand corner and click the Import Collection icon.

### What's in this collection
Essentially it has all of the requests that the REST API can currently make. This is the same list as found in the [Rest API Documentation](http://onlinehelp.tableausoftware.com/v8.2/server/en-us/help.htm#rest_api.htm%3FTocPath%3DREST%20API%7C_____0).

### So how do you use this?
The documentation is your friend. This collection is not a replacement for that, but a convenience for testing out what you learn in the documentation. In addition, there is an online video to assist you in getting started with the REST API. <Video URL to come>

Most calls require IDs for objects. For instance if you want to find out what workbooks were published by a specific user on a specific site, you will need to query the site to find it's id and then you will need to query the users on that site to find the id of the specific user.

All of these functions are present in this collection, but you must replace the authToken and IDs that appear and also the server url/ip to point it at your installation of Tableau Server.