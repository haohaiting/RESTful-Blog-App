# :metal: RESTful Blog App

A RESTful blog web application using NodeJS, expressJS, MongoDB, Semantic UI...

Packages:
```
    npm install body-parser ejs express express-sanitizer method-override mongoose
```

## :sparkles: Look

![blogs](/img/blog.png)
![newblog](/img/newblog.png)

## :+1: REATful Routs
> A table for all 7 RESTful routes

Name    | Path	            | HTTP verb	| Purpose | Mongoose Method
------- | ----------------- | --------- | ------- | ---------------
Index	| "/blogs"	        | GET	    | List all the blogs	                            | Blog.find()
New	    | "/blogs/new"	    | GET	    | Show the form to post a new blog	                | N/A
Create	| "/blogs"	        | POST	    | Create the new blog, then redirect to somewhere	| Blog.create()
Show	| "/blogs/:id"	    | GET	    | Show the details of a specific blog	            | Blog.findById()
Edit	| "/blogs/:id/edit"	| GET	    | Show edit form of a specific blog	                | Blog.findById()
Update	| "/blogs/:id"	    | PUT	    | Update a particular blog, then redirect to somewhere	| Blog.findByIdAndUpdate()
Destroy	| "/blogs/:id/"	    | DELETE	| Delete a particular blog, then redirect to somewhere | Blog.findByIdAndRemove()