PHP:
Redis, node.js, API, OOPs, 

UAT/Production environments



phpdocblog

swagger 

OOPs:
 OOPS concepts
   Class & Objects 
   Specifiers 
   Abstraction  
   Encapsulation 
   Inheritance
   Interfaces
   Abstract Classes
   Overloading
   Overriding
   Traits
   
When should i use static methods?
   
   
__call
   
   
   Magic Methods:
    __construct, __destruct, __get , __set, 
   Magic Constant: magical constants i.e. values that change depending on where they are used
   __LINE__, __FILE__, __CLASS__, _-FUNCTION__, __TRAIT__, __METHOD__, _-NAMESPACE__

   SUPER GLOBALS: $GLOBALS, $_SERVER,  $_REQUEST, $_POST, ..etc
   Final Keyword
   Static Keyword

- A class can have both static and non-static methods. 
  A static method can be accessed from a method in the same class using the self keyword and double colon (::):   

-Magical method in a class must be declared public.
   
   Type declaration:  define the type of the parameter
	
Design patterns
 - singleton desin pattern
 - Factory design pattern
Diff etween session & cookie
XSS attacks and CSRF(cross site request forgery) attacks 
how to debug php code (xdebug)
performance of website (query optimization, code optimization , images loading & minimized libraries)
try/catch/finally blocks
Helper / Libraries / Plugin
Cache (memcache) & redis  
Authentication & Authorisation
How to sanitize your inputs before submitting the data to the database
Diff between constant & global/session variable?
What are getters and setters and why are they important?
Date & Time 

How many ways can you change PHP configuration

proceddure oriented function
class
plugins on top of that input and output 

observer design pattern


SQL:
diff between stored procedure and function
Why we use PDO
aggregate functions
Transaction
ACID properties
  

Diff between padding margin

what are the Webhooks  (call back mechanism )
Cronjobs

Tilio library 
set classes and function which will serve the particular functionalities


Rest Services

cURL

swagger

Content-Type: application/json
At server side, an incoming request may have an entity attached to it. To determine it’s type, server uses the HTTP request header Content-Type. Some common examples of content types are “text/plain”, “application/xml”, “text/html”, “application/json”, “image/gif”, and “image/jpeg”.

https://restfulapi.net/http-methods/

HTTP Method	CRUD	Entire Collection (e.g. /users)	Specific Item (e.g. /users/123)
POST	  Create	     201 (Created), ‘Location’ header with link to /users/{id} containing new ID.	Avoid using POST on single resource
GET	      Read	         200 (OK), list of users. Use pagination, sorting and filtering to navigate big lists.	200 (OK), single user. 404 (Not Found), if ID not found or invalid.
PUT	     Update/Replace	 405 (Method not allowed), unless you want to update every resource in the entire collection of resource.	200 (OK) or 204 (No Content). Use 404 (Not Found), if ID not found or invalid.
PATCH	  Partial Update/Modify	405 (Method not allowed), unless you want to modify the collection itself.	200 (OK) or 204 (No Content). Use 404 (Not Found), if ID not found or invalid.
DELETE	  Delete	     405 (Method not allowed), unless you want to delete the whole collection — use with caution.	200 (OK). 404 (Not Found), if ID not found or invalid.

> What is the use of Accept and Content-Type Headers in HTTP Request? 
> what are the HTTP methods supported by REST? (GET, POST, PUT, DELETE, OPTIONS, HEAD)
> What are the best practices to create a standard URI for a web service? 
> What is the purpose of HTTP Status Code? (refers to predefined status of task done at server.)(200, 201, 400, 401, 404, 500)
> What are the primary security issues of web service? (Confidentiality, Network Security, authentication)

allowing all the domians to access web service

check that user is valid user or not - authentication
having proper permissions to access the particular information - authorization

POST is always for creating a resource ( does not matter if it was duplicated )
PUT is for checking if resource is exists then update , else create new resource
PATCH is always for update a resource



csrf token
json web token
validate that all inputs sanitization 
proper headers and return types
handle exceptions
SQL injections
encryption & decrypt
md5/algorithm

https - security certificate--secure way of connecting between 

70


Accept headers tells web service what kind of response client is accepting, so if a web service is capable of sending response in XML and JSON format and client sends Accept header as application/xml then XML response will be sent. For Accept header application/json, server will send the JSON response.
Content-Type header is used to tell server what is the format of data being sent in the request. If Content-Type header is application/xml then server will try to parse it as XML data. This header is useful in HTTP Post and Put requests.


> Use Plural Noun − Use plural noun to define resources. For example, we've used users to identify users as a resource.
> Avoid using spaces − Use underscore(_) or hyphen(-) when using a long resource name, for example, use authorized_users instead of authorized%20users.
> Use lowercase letters − Although URI is case-insensitive, it is good practice to keep url in lower case letters only.
> Maintain Backward Compatibility − As Web Service is a public service, a URI once made public should always be available. In case, URI gets updated, redirect the older URI to new URI using HTTP Status code, 300.
> Use HTTP Verb − Always use HTTP Verb like GET, PUT, and DELETE to do the operations on the resource. It is not good to use operations names in URI.

$array1 = array(0, 1, 2);
$array2 = array("00", "01", "2");
$result = array_diff_assoc($array1, $array2);  // array(0, 1)

$rest = substr("abcdef", -2);   // ef
null coalcase

array(1, 2, 3) -> array(1, 8, 27);

$a = '1';
$b = &$a;
$b = "2$b"; 
echo $a.", ".$b;    // 21, 21

 Difference between CHAR and VARCHAR?
 
 

Convert a JavaScript object into a string with JSON.stringify().
Parse the data with JSON.parse(), and the data becomes a JavaScript object.

htmlspecialchars & htmlentities




Encapsulation can be achieved by Declaring all the variables in the class as private and writing public methods in the class to set and get the values of variables.
Encapsulation solves the problem and issue that arise at the implementation stage.
Encapsulation enables you to hide the code and data into a single unit to secure the data from the outside world.
You can implement encapsulation using Access Modifiers (Public, Protected & Private.)


Abstraction solves the problem and issues that arise at the design stage.
Abstraction allows you to focus on what the object does instead of how it does it
abstraction can achieve using Interface and Abstract Class.

Abstraction shows only useful data by providing the most necessary details whereas Encapsulation wraps code and data for necessary information.

Backend API
HLD, 
Code sniffer, VS 
Sonar cube

How to debug, docKer environm
sumo logic
timezone issues


MySQL+MoongoDB


stateless architecture - 




URI 
 - resource
 - 

 mapping to active record  row to the class
 

PHP 7 features:
 excel library
 execution time less
 optimization techniques
 diff libraries
 traits - inheritance
 
 
 


CSRF token: 
debug: logs, try,catch, finally, http handler, sonar cube tool, PHPUnit test, 

	apache logs, cloud logs, 	
	
static method - speed execution, no object creation

helpers - functions
libraries - classes
plugins -
	
	
----------------------
Laravel

	
What is use of the header() function in PHP?
	
header() is used to redirect from one page to another: header("Location: index.php");
header() is used to send an HTTP status code: header("HTTP/1.0 this Not Found");
header() is used to send a raw HTTP header: header('Content-Type: application/json');

Explain Migrations in Laravel?
Laravel Migrations are like version control for the database, allowing a team to easily modify and share the application’s database schema. Migrations are typically paired with Laravel’s schema builder to easily build the application’s database schema.

What is Eloquent Models?
The Eloquent ORM included with Laravel provides a beautiful, simple ActiveRecord implementation for working with your database. Each database table has a corresponding Model which is used to interact with that table. Models allow you to query for data in your tables, as well as insert new records into the table.

The "Laravel service container" is a tool for managing class dependencies and performing dependency injection.

What is the Facade Pattern used for?

	Facades provide a static interface to classes that are available in the application's service container. Laravel facades serve as static proxies to underlying classes in the service container, providing the benefit of a terse, expressive syntax while maintaining more testability and flexibility than traditional static methods.

	All of Laravel's facades are defined in the Illuminate\Support\Facades namespace. Consider:

	use Illuminate\Support\Facades\Cache;
	Route::get('/cache', function () {
		return Cache::get('key');
	});
	
	What is service provider/ Service container
	

Names routes and Resource Routes

What are named routes in Laravel?
	Named routes allow referring to routes when generating redirects or Url’s more comfortably. You can specify named routes by chaining the name method onto the route definition:

	Route::get('user/profile', function () {
		//
	})->name('profile');
	You can specify route names for controller actions:

	Route::get('user/profile', 'UserController@showProfile')->name('profile');
	Once you have assigned a name to your routes, you may use the route's name when generating URLs or redirects via the global route function:

	// Generating URLs...
	$url = route('profile');

	// Generating Redirects...
	return redirect()->route('profile');


Accessors =>  create a get{Attribute}Attribute method on
mutators => To define a set{Attribute}Attribute method on your model where {Attribute} is the "studly" cased name of the column you wish to access

How to send notifications?
notify method or Notification facade

CORS issue

Service Provider Concept
  - central place to configure your application.
  - registering things, including registering service container bindings, event listeners, middleware, and even routes. 
  - Register and boot method
  

Events & Listeners Concept:
Facades concepts
Facades vs Dependency Injection


If your Service doesn’t accept any parameters while creating its object new ReportService(), then just use static methods. You don’t need to create an object, at all.


If possible,

How do you do soft deletes?
or
what is soft delete



Restful Services
Resource Controllers


---
tabula
Icharts in javascript


foundation components

Macro in netbeans

google g-metrics

amp pages
seo score
gsip 
