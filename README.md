# reduxProfitabilityCalc
The Overdrive Challenge

The Overdrive Challenge
Required Stack
Back-end: NodeJS, ExpressJS
Front-end: React (redux optional)
Data-tier: MYSQL (sequelize integration)
Deployment
AWS EC2 with Amazon Linux or Ubuntu @ latest (currently 16.02)
MYSQL (Deployed in AWS RDS or installed on the EC2 instance)

The Overdrive challenge is an opportunity for prospective developers to show their skills, and get a feel for the type of work we do.  The Overdrive challenge will explore your ability as a Javascript developer.  We don’t expect you to be a pro at all the technologies that we use, but we are a team of learners and innovators and we often must learn on the fly with little to no supervision.  
Completing the challenge will show us that even if you don’t have experience with all the tools you can adapt and grasp new technologies.  The ability to learn while doing to complete the project is a key competency at Overdrive Brands.
You will be responsible for building a product profitability calculator.
Project Overview
This app consists of three major elements
Home page
This page is used for display a list of current products and navigating to subsequent pages
New Item page
This page will contain an interactive form that will allow a user to POST a new product into inventory (and adding it to current products)
Calculator Screen
This page contains a semi-interactive form where a user can test the pricing of a product and view profitability at certain points.

You will be responsible for building both the back-end RESTful API using NodeJS and ExpressJS with an integration to a MYSQL database and a react based front end web app with the following functionality:
From the home screen a user can click a button to add a new item new item screen
From the home screen a user can click on a product that has already been created to move to a calculator screen
The home screen should also provide a link for the user to remove the sku from the database (but should prompt the user to confirm he/she meant to delete the item).
The home screen should provide a link to edit the sku in the same manner as the new item screen
The new item screen should consist of a simple form that allows the user to input a SKU, Item Name, Product Cost, and Expected Freight.
The Calculator Screen should consist of a form that pulls the given SKUs data (per above) into a form that the user can manipulate (Cost and Freight) plus an additional input box for price and a calculation for Expected Profit and Profit Margin (see attached excel sheet for wireframe and usability)
When the user makes a change to the Cost, Freight, or Price fields the page should recalculate the expected profit and profit margin.
You should also include some navigation to navigate back to the home screen from the calculator and new item screen

API Routes (suggested – you should use whatever nomenclature makes sense to you)
GET product/ - list all created products
POST product/ - add a new product
GET product/<SKU> - get a specific product (for edit or calculator)
PUT product/<SKU> - update a specific product
DELETE product/<SKU> - remove a specific product

React App pages/components (again, name them however you think you should)
Home – list all products
Add – add a new product (can also be used to edit the item if you want to reuse the component)
Edit – edit a product (if you don’t want to reuse the above component)
Calculator – allow the user to play around with pricing on the item

Resources
ExpressJS
https://expressjs.com/
https://scotch.io/tutorials/build-a-restful-api-using-node-and-express-4
Sequelize (Data relational Mapper)
http://docs.sequelizejs.com/
http://www.tothenew.com/blog/nodejs-with-mysql/
React
https://facebook.github.io/react/
https://github.com/facebookincubator/create-react-app
This generator manages your webpack integration so you don’t have to.  You don’t have to use it, but it does make it easier and faster to get an app going.
React Router
Important note:  The most recent version of React-Router (v4) is a complete rewrite so if you know v2 or v3 it will be very different from most recent version.  You can use whatever version you are comfortable with.
https://github.com/ReactTraining/react-router
React/Bootstrap
https://react-bootstrap.github.io/
Provides pre-made bootstrap components for React, not required, but an option if you want to use it.
Redux
Redux is a state (data) container for web apps and it pairs nicely with React.  Essentially, React listens data updates from Redux and automatically rerenders the DOM.  Using Redux isn’t required, but it does make managing data much easier.
http://redux.js.org/
https://scotch.io/tutorials/build-a-bookshop-with-react-redux-i-react-redux-flow
Axios
Axios is a lightweight AJAX library for front-end development
https://www.npmjs.com/package/axios

AWS EC2
https://scotch.io/tutorials/deploying-a-mean-app-to-amazon-ec2-part-1
http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EC2_GetStarted.html

AWS Security Groups (Virtual Firewall)
http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using-network-security.html

AWS RDS (MySQL)
http://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/CHAP_GettingStarted.html
http://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/TUT_WebAppWithRDS.html



