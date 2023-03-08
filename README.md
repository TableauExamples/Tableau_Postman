  <br/>

> ![This repo is not maintained](/warning_icon.png)<br/> <br/>Instead, try the **[Tableau REST API collection](https://www.postman.com/salesforce-developers/workspace/salesforce-developers/collection/12721794-7d783742-165f-4d10-8c4c-5719fb60fba2)** in the Salesforce Developer Postman workspace. This new collection is an up to date, community supported resource containing requests for each method, preconfigured with environment variables and other conveniences.<br/><br/> See [How to Use the Collection](https://github.com/tableau/tableau-postman/blob/main/README.md#how-to-use-the-collection) to get started. <br/><br/>

<br/>
____________________

<br>


## Postman Collection for Tableau's REST API for Tableau 10.0 (v2.3)

There are two .json files for importing into [Postman](http://www.getpostman.com/), a tool for making HTTP requests via the browser.

To import, open Postman, click on the Collections tab in the upper-left hand corner and drag/drop or select the two files and click Import.

### So how do you use this?
The documentation is your friend. This collection is not a replacement for that, but a convenience for testing out what you learn in the documentation. In addition, there is an [online video to assist you in getting started with the REST API.](https://www.tableau.com/learn/tutorials/on-demand/rest-api)

### What's in this collection
Essentially, it has all of the requests that the REST API can currently make. This is the same list as found in the [Rest API Documentation]( https://onlinehelp.tableau.com/current/api/rest_api/en-us/help.htm).

#### API Examples
The API examples file has the API calls in it.  It also has two example workflows that you can follow for On-boarding (creating users and add to groups) and Content Management (copy project and set permissions).

#### Environment Variables
New since the 9.0 release, Postman now allows environment variables.  This is useful when stringing together API calls.  They allow automatic (or with manual intervention) assigning of variables that can be re-used.  An example is signing in.  Upon sign in, the user is provided an API token that needs to be added to the headers for all subsequent calls.  The Postman "Tests" will automatically assign this to an environment variable so you do not need any manual intervention.  Environment variable are represented like <code>{{server}}</code>.

<b>When do you need manual intervention with the environment variables?</b>
Typically, (but not always), when there is a single or very few responses to a request they will be extracted.  When there are numerous objects returned is when you should manually set the variables.  For example, querying the server for a list of users will provide many different responses back.  In this case, you will need to highlight the ID of the object and set this (right click context menu=>set...) to userID and the name of the user to userName.  Clicking the "eye" in the upper-right will reveal the environment variables.  (Hint: the API never uses the literal strings, but setting them at the same time as the ID will let you quickly identify what ID is referenced.)    

### Updated for 10.0 (v2.3)
10.0 further builds upon the REST API and supports revisions, data sources, schedules, and more.  To see a complete list of new features by release, read the [what's new.](https://onlinehelp.tableau.com/current/api/rest_api/en-us/help.htm#REST/rest_api_whats_new.htm)

### Updated for 9.0 (v2.0)
9.0 added many useful functions to the REST API including Project management, Group management, Permissions management, downloading, publishing, and more. This collection has been updated to reflect those changes.

### Multi-part forms
Note: The functions for publishing are in this collection, but POSTman will set the content-type to multipart/form-data, while the api is expecting multipart/mixed. So for using POSTman to test publishing, you can make the request from POSTman, it will fail, but then you can open the request in an application like Charles or Fiddler, modify the request to change it to multipart/mixed and it should work.
Here is a [video on how to use POSTman plus Charles or Fiddler to publish.](http://youtu.be/hiYaekLuV4Q)  (This video is from the 9.0 collection, but the techniques are still valid.)

### Warning
This collection is not officially 'blessed' by Tableau Engineering or Support.
What does that mean? We didn't have a qa team test it. It's a tool for learning how to use the REST API and shouldn't be used for more than that.
You should not expect that there are 0 bugs.

If you have problems getting it to work, feel free to Email us with questions, but we won't promise quick responses.

Sorry =)
