# Bloggy

- [What is Bloggy?](##what-is-bloggy)
- [Completed Requirements](##completed-requirements)
- [Tech Stack](##tech-stack)
- [Above and Beyond Features](#above-and-beyond)
- [Next Steps](#next-steps)
- [Contributions](#contributions)

## What is Bloggy?

![Bloggy banner](./assets/banner/banner.png)

> Bloggy is a content-sharing web platform in which bloggers can publish blogs and readers can read and comment on blogs.


## Completed Requirements

### Minimal requirements

- [x] Publisher
  - [x] Can register and log in
  - [x] Can create and edit articles in a markdown rich text editor
  - [x] Can switch between source code mode and preview mode in the editor
  - [x] Can delete and respond to comments

- [x] Reader
  - [x] Can register and log in
  - [x] Can read articles
  - [x] Can like articles
  - [x] Can post comments to articles

### Standard requirements

- [x] Publisher
  - [x] Can post and edit projects
  - [x] Can save unpublished articles as drafts

- [x] Reader
  - [x] Can view projects

### Stretch requirements

- [x] Publisher
  - [x] Can assign tags to articles
  - [x] Can create an about page and edit it

- [x]  Reader
  - [x] Can filter articles by tags
  - [x] Can filter articles by year  
  - [x] Can view the about page

## Tech Stack

## Above and Beyond Features

- Fully Responsive

> Bloggy provides excellent user experience for both desktops and mobile devices. To achieve this feature, we have designed and implemented two separate sets of components to support each platform.

- Fully Accessible

> Bloggy is fully accessible as it provides special theme called 'color weakness mode' to make the web site usable by everyone, regradless of their ability or disability.

- Coherent and Customizable UX design

> Our team follows a coherent style througout the design and implementation which provides better user experience. Bloggy also enables users to customize the themes accroding based on preferences. T

- Multiple Languages

> Bloggy supports both English and Chinese as they are widely-used languages around the world which helps the application to expand the user population.

- Lazy Loading

> This is a speical algorithm we designed for the better performance of front-end rendering . For example, if there are 1000 blog posts in the database, the frontend will not render all the posts at once. Instead, it will render the first five posts first and render more when users further request

- Safe Authentication

> Instead calling third-party API for user login, our team implemented a safe authentication feature using web token.  This feature is beneficial for maintainability as thrid-party APIs may change.

## Next Steps

- Frontend Testing

> Due to time constraint, we are unable to test frontend systematically.  In the future, our team will implement a test suite which could generate mock data for frontend so that the front-end development could progress independently from backend.

- Third-Party Login

> It is convenient for users if the application supports third-party login.  In the future, we may consider implement this feature to allow users login into our applicaiton through Google or Github.

## Contributions

- Chuntong Gao (Tech Lead)

> Chuntong is the tech lead in the team as he has the expertise in web development.  He clearly set the requirements and decided technologies used in the application.  He contributed both frontend and backend as well as solved many challenge problems througout the term.

- Bolin Wang (developer)

> Bolin is the backend developer in the team. She mainly worked on the the CRUD operations with typescript. She also drawed the prototypes of our appliation.

- Kerry Zhou (developer)

> Kerry is the frontend developer in the team. He mainly worked on the UI components and styles of the application. He was also responsible for the deployment of the application.

- Max Song (developer)

> Max is the frontend developoer in the team. He mainly works on the UI components and interfaces used to connect backend.  He was aslo responsible for the documentation and project management in the team.