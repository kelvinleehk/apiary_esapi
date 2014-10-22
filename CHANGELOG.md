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
