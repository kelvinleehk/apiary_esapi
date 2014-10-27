## 2014-10-27
* Add notificaiton settings API
* Add bug report API
* Force fbToken key to be string by adding double quotes around theme
* Add paginations to event and user queries
* Update user query collection parameter descriptions

## 2014-10-23
* Remove bookmark event
* Fix incorrectly named search event endpoint

## 2014-10-22
* Add user query status legend to blueprint
* Change user query APIs to use query parameters
* Change event query APIs to use query parameters
* Add new events API
    * Upcoming events
    * Attending
    * Attended events
* Add new friends API
    * Following users
    * Users who follow
    * PLURed
    * Not connected users

### 2014-10-20
* Added Bookmark event endpoint
* Added Remove Event endpoint
* Changed all IDs to be using ObjectId instead of numeric IDs
* Changed login to use fb token
* Changed all images to use absolute path instead of relative path
* Changed event and user profile image uploading input to be BLOBs
* Removed userId from endpoints where it relates to the logged in user:
	* /user/{userId}/image is now /user/image
	* /user/logout is parameterless and only requires the token
	* /user/{userId}/is_admin is now /user/is_admin
	* /users no longer requires the userId parameter
	* /events no longer requires the userId parameter
