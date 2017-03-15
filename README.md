# Angular Freezedry

System for pre-rendering ('server side rendering') pages at build-time so your server can be a dumb box again.

## Requirements
Freezedry expects a build environment as if you were making a seperate server and client build. 

## Usage
	freezedry dist/server.js ["/", "/kittens", "/about"]

output:

	index.html
	kittens.html
	about.html

or simply:
	
	freezedry dist/server.js

outputs only `index.html`.

Remove these from your serverside 'catch all' that rewrites all urls to load index.html.

## Credits
- Thought up in a workshop by [Manfred Steyer](https://github.com/manfredsteyer/)
- This is based on a fork of the well-known library [ngx-translate](https://github.com/ngx-translate/core) that uses its project setup.
