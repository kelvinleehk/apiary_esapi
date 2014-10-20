### 2014-10-20
* Changed login to use fb token

### 2014-10-13
* Removed userId from endpoints where it relates to the logged in user:
	* /user/{userId}/image is now /user/image
	* /user/logout is parameterless and only requires the token
	* /user/{userId}/is_admin is now /user/is_admin
	* /users no longer requires the userId parameter
	* /events no longer requires the userId parameter