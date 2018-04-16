# RESTful Web Service

##Social Media Application

###User 1--* Posts

- Retrieve all Users			- GET /users
- Create a User				- POST /users
- Retrieve one User			- GET /users/{id} -> /users/1
- Delete a User				- DELETE /users/{id} -> /users/1

- Retrieve all posts for a User   - GET /users/{id}/posts
- Create a post for User		     - POST /users/{id}/posts
- Retrieve details of a post		 - GET  /users/{id}/posts/{post_id}


#### Internationalization

##### Configuration
- LocaleResolver
	- Default Locale - Locale.US
- ResourceBundleMessageSource

##### Usage
- Autowire MessageSource
- @RequestHeader(value = "Accept-Language", required = false) Locale locale
- messageSource.getMessage("HelloWorld.message", null, locale)