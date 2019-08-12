---
sitemap: false
excerpt: "Nicole Weatherburne Projects"
permalink: /projects.html
date: 2019-08-10
---

<h1>XML file parser service</h1>
This service searches for special XML Configuration files from a defined location and parses them every hour. Files go through a number of validations and then processed accordingly.
<br><br>Major features:
<br>- Refactored code to allow switching out any part of the tech stack if necessary
<br>- Setup Celery Flower plugin in order to monitor worker uptime and jobs processed
<br>- Use ElementTree library for parsing XML
<figure>
<a href="images/xml-conf-parser-architecture.jpg"><img src="images/xml-conf-parser-architecture.jpg"></a>
<figcaption>XML Configuration parser Architecture</figcaption>
</figure>

<br><br>

<h1><a href = "https://github.com/wisebits">Wisebits URL Shortner</a></h1>
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

<h1><a href = "https://github.com/ZhongMeiZhou">TraViz</a></h1>
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

<h1>Coral Bleaching Information System</h1>
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

<h1><a href = "https://github.com/Hopenglish-Miners">Hopenglish Miners</a></h1>
The dataset was provided by an e-learning company based in Taiwan. Their online e-learning platform provides different alternatives to efficiently learn the English language through the use of multimedia content, such as video clips and audio recordings. The dataset consisted of video details and student behaviours which show how students interacted with videos. We were asked to discover some interesting insights that we can provide to the company to better understand their clients and improve their service. After gaining extensive insights into the data, we found a pattern in the student behaviour which could eventually lead to students quitting the service. We performed a classification using a decision tree to perform a prediction in an effort to identify when students lose interest. Our argument is that if we can identify when students lose interest, the company can recommend better videos that could keep the users engaged and reduce student dropout. We developed a web application to demonstrate the real world application of our proposal.
<br><br>Major Features/Tasks:
<br>- Data Exploration/Visualization (Pandas, Jupyter, K-means clustering algorithm, Plotly)
<br>- Data pre-processing (Feature selection/creation to address curse of dimensionality problems - clustering algorithms)
<br>- Data mining algorithm (Supervised algorithm to perform classification: C4.5 Decision Tree - 70% training/30% testing using WEKA)
<br>- Data mining evaluation (10 Fold Cross Validation with 64% accuracy)


<br><br>

<h1><a href = "https://github.com/rjollet/NeverAloneNTHU">Never Alone Dating Service</a></h1>
We developed a dating service that recommends potential matches to users. We used Django Framework and Neo4J Graph Database. We wrote recommendation algorithms and made use of concepts such as Jaccard Similarity in order to recommend matches based on similar interests.
<br><br>Major Features/Tasks:
<br>- Built a recommendation algorithm
<br>- Use Django authentication


<br><br>

<h1>Passtime Projects</h1>
<div class="panel panel-primary">
      <ul class="list-group">

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
<br>- Booking app to better connect users and businesses
<br>- Homework correcting system
<br>- Neighbourhood watch app - The idea of this is to allow community residents to report crime in their area anonymously
<br>- Visualization of Github Jobs
<br>- Detect emotion level of posts
