# Bloggy 

## https://bloggy2020.herokuapp.com

This repo mainly provides an overview for the Bloggy project. If you are looking for source code, please refer to the following links:

- [Back-end repo](https://github.com/chuntonggao/bloggy-server.git) 
- [Front-end repo for publisher view](https://github.com/chuntonggao/bloggy-publisher.git)
- [Front-end repo for reader view](https://github.com/chuntonggao/bloggy-reader.git)

- [What is Bloggy?](##what-is-bloggy)
- [Features](##features)
- [Tech Stack](##tech-stack)
- [Above and Beyond Features](#above-and-beyond)
- [Next Steps](#next-steps)
- [Contributions](#contributions)

## What is Bloggy?

![Bloggy banner](./assets/banner/banner.png)

> Bloggy is a content-sharing web platform in which bloggers can publish blogs and readers can read and comment on blogs.

## Features

### Minimal requirements

- [x] Publisher
  - [x] Can register and log in
  - [x] Can create and edit articles in a markdown rich text editor
  - [x] Can approve and delete comments
  - [x] Can update personal information
  - [x] Can jump to the reader view by clicking on a link
  - [x] Can view all articles in list mode and see stats (view, likes & comments)

- [x] Reader
  - [x] Can register and log in
  - [x] Can view the author's home page
  - [x] Can view the author's articles in list mode
  - [x] Can read articles in article mode
  - [x] Can post comments to articles

### Standard requirements

- [x] Publisher
 - [x] Can switch between source code mode and preview mode in the editor
 - [x] Can create categories and assign categories to articles
 - [x] Can set article to draft/public mode to hide/show the article

- [x] Reader
  - [x] Can filter articles by categories
  - [x] Can like articles (duplicate likes not allowed)
  - [x] Can click on the profile link of a comment, to see the blog of the commenter 
 
### Stretch requirements

- [x] Publisher
  - [x] Can toggle between light/dark mode, choose a main theme colour and switch layout
  - [x] Can switch between language (currently English and Chinese)
  - [x] Can set an about-page to introduce the blog author

- [x]  Reader
  - [] Can filter articles by year  
  - [x] Can view the about page

## Tech stack

### Unit 1 - HTML, CSS, JS && Unit 2 - React & Redux

Our front end is written in TypeScript and React. React enables us to make modular components. For example, a menu bar can be seen as a separate component. Since we used JSX syntax, we did write much HTML code in our project. However, JSX resembles HTML a lot, and our knowledge about HTML is transferrable to writing JSX elements. We also used CSS preprocessors SCSS and Less to style our front end. SCSS and Less have all features that CSS has, but also have additional features like functions, nesting and variables.

We also integrated Redux into React. Redux allows to handle state changes globally using reducers and actions. However, since reducers are pure functions, handling async requests can be tricky in Redux. To handle async requests, we integrated redux-saga and redux-thunk.

We used axios for sending HTTP requests. The front end performs CRUD operations by sending HTTP requests to the back end and fetching data from the back end.

### Unit 3 - MongoDB

We stored all our data as documents in the document-based databased MongoDB. Compared to traditional relational databases, MongoDB is more flexible and the document format closely resembled JavaScript objects. We made schemas for our users, articles, categories and comments. Each schema has several properties and restrictions. We also used Mongoose framework to better connect our Node.js back end with MongoDB.

### Unit 4 - Node & Express

We implemented our back end with Node.js and TypeScript. We also used Express.js as our RESTful framework. Our back end provides several endpoints for CRUD operations, which the front end can access through HTTP requests. In case of errors, our back end also provides meaningful error messages and status codes (like 404 for not found, 400 for not authorized). We also tested our back end with 95% coverage with Mocha, Chai and Supertest. Testing is fully automated and run on every commit/push.

### Unit 5 - Release Engineering

We set up CI/CD pipelines with Travis CI. On every push, code style will be checked and tests will be run. If CI/CD passes, the pushed code will be released into production. We deployed our app into Heroku. Heroku is a deployment platform which can be connected to our GitHub Repos. Heroku also provides us with some metrics like response times and volumes, which give us insight into user behaviour.

## Above and Beyond Features

### Fully Responsive
First, as you have seen, Bloggy is fully responsive. We designed mobile-specific UI components instead of just scaling down the desktop view. 

### Fully Accessible
Bloggy provides a colour theme for people who have difficulty distinguishing colours. It also supports screen readers to help visually challenged users.

### Highly Customizable
Users can customize themes. They can toggle light / dark mode, choose the main theme colour and change layout. Users can also switch languages. We currently support English and Chinese, but other languages can be easily integrated.

### Lazy Loading
We designed a lazy-loading algorithm to improve front-end performance and experience. For example, if there are 1000 blog posts in the database, the frontend will not fetch and render them all. Instead, it will fetch and render the first five. When the user scrolls to the bottom, the next five will be loaded.

## Next Steps

- Frontend Testing

> Due to time constraint, we are unable to test frontend systematically.  In the future, our team will implement a test suite which could generate mock data for frontend so that the front-end development could progress independently from backend.

- Third-Party Login

> It is convenient for users if the application supports third-party login.  In the future, we may consider implement this feature to allow users login into our application through Google or Github.

## Contributions

- Chuntong Gao

> Chuntong set up the scaffolding for the project as he has the expertise in web development. He clearly set the requirements and decided technologies used in the application.  He contributed both frontend and backend as well as solved many challenging problems throughout the term.

- Bolin Wang 

> Bolin is the backend developer in the team. She mainly worked on the the CRUD operations with typescript. She also drew the prototypes of our.

- Kerry Zhou

> Kerry is the frontend developer in the team. He mainly worked on the UI components and styles of the application. He was also responsible for the deployment of the application.

- Max Song

> Max is the frontend developer in the team. He mainly works on the UI components and interfaces used to connect backend. He was also responsible for the documentation and project management in the team.
