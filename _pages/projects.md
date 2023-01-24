---
sitemap: false
excerpt: "Nicole Weatherburne Projects"
permalink: /projects.html
date: 2020-05-25
---

<h1><a href = "https://github.com/nweat/udemy-course-tracker">Udemy Bot (2020)</a></h1>
Built an FB messenger bot for the purpose of checking for content updates for paid Udemy courses. It also checks when there are discounts for courses I would like to buy. The RESTFul API was built using Node.js/Express and is hosted on Heroku. Webhooks enable the seamless integration between the API and the FB Messenger Platform. 
<figure>
<a href="images/snapshot.PNG"><img src="images/snapshot.PNG"></a>
<figcaption>FB Bot</figcaption>
</figure>

<br><br>

<h1>Wafer Map Visualizer (2020)</h1>
In the semiconductor industry, a wafer map is used to represent the performance of semiconductor devices. Each tested die is assigned a bin value depending on the test result. Bins are represented by different colors making it easy for engineers to visualize product test results and recognize failure patterns. 
The reason for the architecture explained below is primarily to handle products with high gross dies per wafer.

<br>Major Features:
<br> - Using Redis Queue (RQ), wafer and chart data can be broken into chunks and pre-processed in background jobs. Job results are kept in Redis which allows RQ to serve as a caching mechanism as well.
<br> - In the front end, <a href = "http://oboejs.com/">Oboe.js</a> consumes job results stored as JSON and streams it to the front end, allowing visualizations to be drawn incrementally. This improves the perceptual performance for users because the user does not have to wait until all the data is available to start seeing the visualizations.

<br>Tech stack:
<br> - Pandas
<br> - Matplotlib
<br> - D3.js
<br> - Highcharts
<br> - Redis Queue (Python RQ)
<br> - Flask/Gunicorn
<br> - NGINX

<figure>
<a href="images/wafer_gallery.png"><img src="images/wafer_gallery.png"></a>
<figcaption>Wafer Map Visualizer</figcaption>
</figure>

<br><br>

<h1><a href = "https://pure-spire-72385.herokuapp.com/">QuickCampaign (2020)</a></h1>
The goal of QuickCampaign is to allow registered users to create Email campaigns that can be sent to many users in a time. Email responses are captured and the application provides an interface where you can visualize user responses. This is particularly useful when you are looking to get feedback on something or just need to send out a survey. 
<br>
<a href = "https://github.com/nweat/QuickCampaign">Github</a> 
<figure>
<a href="images/quickcampaign.png"><img src="images/quickcampaign.png"></a>
<figcaption>QuickCampaign</figcaption>
</figure>

<br><br>

<h1>Wafer inking service (2019)</h1>
Developed a React web application that allows users to upload wafer configuration data. The wafer configuration is applied to a wafer map which involves performing manipulations on large amounts of data. This process is part of the wafer testing process. 
<figure>
<a href="images/geoink.png"><img src="images/geoink.png"></a>
<figcaption>Wafer inking service Architecture</figcaption>
</figure>

<br><br>

<h1>XML file parser service (2018)</h1>
This service searches for special XML Configuration files from a defined location and parses them every hour. Files go through a number of validations and then processed accordingly. I needed to deploy a stable service that is able to process large amounts of files in less time. After lots of reading blogs and recommendations from the Python community I decided to go with this setup. 
<br><br>Major features:
<br>- Refactored code to allow switching out any part of the tech stack if necessary
<br>- Setup Celery Flower plugin in order to monitor worker uptime and jobs processed
<br>- Use ElementTree library for parsing XML
<figure>
<a href="images/otp.png"><img src="images/otp.png"></a>
<figcaption>XML Configuration parser Architecture</figcaption>
</figure>

<br><br>

<h1><a href = "https://github.com/wisebits">Wisebits URL Shortner (2017)</a></h1>
Developed a secured service that allows authorized users to generate and share shortened URLs. Registered users can create a shortened URL that is secure and shareable among users with appropriate permissions. The service was built in Ruby (Sinatra) using Slim and Bootstrap for the client application. We used heroku and postgres to host our services and databases. We made use of <a href = "https://github.com/cryptosphere/rbnacl">Rbnacl</a> cryptographic libraries for implementing security features.
<br><br>Gained experience in developing a secured distributed architecture which included:
<br>- Securing databases through SQL injection, mass assignment restrictions, ORM based encryption
<br>- User Authentication
<br>- Password hashing (Salt + Hash + Key stretching)
<br>- Token based Authentication (secured session and cookies, safe user registration and authorization)
<br>- Token based Authorization (Signed client apps (JWK), secure API requests)
<br>- OAuth Authorization Protocol
<br>- Preventing XSS/CSRF attacks, protecting HTTP headers
<br>- API and interface testing
<br>- Defining access control
<br>- Enforce SSL/TLS
<figure>
<a href="images/ss.png"><img src="images/ss.png"></a>
<figcaption>URL Shortner Service Architecture</figcaption>
</figure>

<br><br>

<h1><a href = "https://github.com/Hopenglish-Miners">Hopenglish Miners (2017)</a></h1>
The dataset was provided by an e-learning company based in Taiwan. Their online e-learning platform provides different alternatives to efficiently learn the English language through the use of multimedia content, such as video clips and audio recordings. The dataset consisted of video details and student behaviours which show how students interacted with videos. We were asked to discover some interesting insights that we can provide to the company to better understand their clients and improve their service. After gaining extensive insights into the data, we found a pattern in the student behaviour which could eventually lead to students quitting the service. We performed a classification using a decision tree to perform a prediction in an effort to identify when students lose interest. Our argument is that if we can identify when students lose interest, the company can recommend better videos that could keep the users engaged and reduce student dropout. We developed a web application to demonstrate the real world application of our proposal.
<br><br>Major Features/Tasks:
<br>- Data Exploration/Visualization (Pandas, Jupyter, K-means clustering algorithm, Plotly)
<br>- Data pre-processing (Feature selection/creation to address curse of dimensionality problems - clustering algorithms)
<br>- Data mining algorithm (Supervised algorithm to perform classification: C4.5 Decision Tree - 70% training/30% testing using WEKA)
<br>- Data mining evaluation (10 Fold Cross Validation with 64% accuracy)

<br><br>

<h1><a href = "https://github.com/ZhongMeiZhou">TraViz (2016)</a></h1>
Developed TraViz Web Application and Data API service. TraViz allows users to generate visualizations of lonely planet tour listings based on specified countries, categories and price range. The service was built in Ruby (Sinatra) using Slim and Bootstrap for the client application.
<br><br>Gained experience in developing a service following a modern service oriented architecture design:
<br>- Followed Agile development model
<br>- Ruby gem created for lonely planet web scraping (OGA)
<br>- Continuos integration (Travis CI)
<br>- Continuos deployment (Heroku, Codeship)
<br>- Distributed Postgres database
<br>- Heavy emphasis on testing (Minitest, Stubs)
<br>- Interface design and testing (mobile first interface)
<br>- Data visualization (HighCharts, Chartkick)
<br>- Reactive user experience using background jobs, queues, web sockets, web caching
<br>- Refactored MVC with OOP (service, value, form objects)

<figure>
<a href="images/soa.png"><img src="images/soa.png"></a>
<figcaption>Sample architecture design</figcaption>
</figure>

<br><br>

<h1><a href = "https://github.com/rjollet/NeverAloneNTHU">Never Alone Dating Service (2016)</a></h1>
We developed a dating service that recommends potential matches to users. We used Django Framework and Neo4J Graph Database. We wrote recommendation algorithms and made use of concepts such as Jaccard Similarity in order to recommend matches based on similar interests.
<br><br>Major Features/Tasks:
<br>- Built a recommendation algorithm
<br>- Use Django authentication

<br><br>

<h1>Coral Bleaching Information System  (2014)</h1>
This application was designed to allow for easy management of data (CRUD), perform data analysis and provide insightful visualizations to environmental researchers. The application was built using PHP CodeIgniter framework and JavaScript/JQuery
<br><br>Major Features/Tasks:
<br>- File upload functionality to allow upload of data entry records from custom excel templates
<br>- HighCharts library was used for generating graphs
<br>- Spatial visualization of analysis results was developed using Google Maps, PHP, MySQL, AJAX, XML
<br>- AJAX and JQuery was used for enhanced user experience (DataTables, jQuery datepicker)
<br>- Developed complex SQL queries for generation of analysis reports
<br>- Implemented SQL injection techniques
<br>- User authentication and user access levels were implemented
<br>- Used FPDF PDF generator library to allow users to save reports as PDF files

<figure class="half">
<a href="images/CORAL_2.png"><img src="images/CORAL_2.png"></a>
	<a href="images/Coral_1.png"><img src="images/Coral_1.png"></a>
	<figcaption>The National Coral Bleaching Monitoring Network (NCRMN) Information System provides coral bleaching statistical reports based on defined time periods and locations along the coast of Belize</figcaption>
</figure>

<br><br>

<h1>Passtime Projects/Competitions</h1>
<div class="panel panel-primary">
      <ul class="list-group">

      <li class="list-group-item">
      <b>Know my Wata (2020)</b>
      <br> Submission idea for People's Livelihood Public IOT Data Competition (Taiwan). The goal was to create an application where the community can quickly access relevant information on water sources particularly rivers and reservoirs around them.
      <br> Front end: React/Redux/React-Leaflet/React-Vis
      <br> Back end: Pandas/Flask
      <br> <a href = "https://github.com/nweat/know-your-water"> Github </a>
      <br> <a href = "https://knowmywata.herokuapp.com/"> Heroku </a>
      </li>

      <li class="list-group-item">
      <b>HealthyBites - React/Redux/React Router/Jest (2020)</b>
      <br> Front end design concept of an online store where users can purchase healthy meal options. The goal is to show the power of React and Redux to manage state along with a concrete responsive UI design.
      <br> <a href = "https://github.com/nweat/shopping-cart-react-redux"> Github </a>
      <br> <a href = "https://healthybites.herokuapp.com/"> Heroku </a>
      </li>

      <li class="list-group-item">
      <b>Bday bot - Express/Socket.io/React (2019)</b>
      <br> Design a simple bot that starts a birthday conversation with a given user
      <br> <a href = "https://github.com/nweat/bday-bot"> Github </a>
      </li>

      <li class="list-group-item">
      <b>Node.js/Express and Socket.io (2019)</b>
      <br> Design a chat room application with Node.js and Socket.io
      <br> <a href = "https://github.com/nweat/chat-app-socketio"> Github </a>
      <br> <a href = "https://nw-chatapp.herokuapp.com/"> Heroku </a>
      </li>

      <li class="list-group-item">
      <b>Angular and Bootstrap (2017)</b>
      <br> Design a file uploader with progress bar. This one was just for fun as I was bored at the time! Please feel free to use in your own apps. :)
      <br> <a href = "https://github.com/nweat/angular-bootstrap-upload-with-progress-bar"> Github </a>
      <br> <a href = "http://sample-angular-bootstrap.herokuapp.com/#/"> Heroku </a>
      </li>

      <li class="list-group-item">
      <b>Resource Stop (2016)</b>
      <br> I didn't have a way to manage online resources so I decided to build a simple web application to do this. I decided to use the MEAN stack (Mongo, Express, Angular, NodeJS) because it was getting a lot of attention at the time. There are a lot of plugins available I found was easy to setup. Mongoose and Passport are such examples for database modeling and google authentication respectively.
    		<br><a href = "https://github.com/nweat/resource-stop"> Github </a>
      <br><a href = "https://nikki-resource-stop.herokuapp.com/">Heroku</a>
      </li>

      <li class="list-group-item">
      <b>Simply Chat (2015)</b>
      <br> Developed a simple real-time chat application using the Meteor Real Time Javascript Framework.
      <br> <a href = "https://github.com/nweat/simply-chat"> Github </a>
      <br> <a href = "https://meteor-simple-chat.herokuapp.com/"> Heroku </a>
      </li>

      </ul>

</div>

<br>

<h1>App Ideas</h1>
These are just some ideas sparked from personal experiences:
<br>- Beach Fun and Cleanup - a blossoming idea for a way for tourists to have fun and keeping the environment clean 
<br>- Booking app to better connect users and businesses
<br>- Homework correcting system
<br>- Neighbourhood watch app - The idea of this is to allow community residents to report crime in their area anonymously
<br>- Visualization of Github Jobs
<br>- Detect emotion level of posts
