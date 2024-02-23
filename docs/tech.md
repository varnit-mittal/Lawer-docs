# Components

## Tech stack
<ul>

    <li>flutter</li>
    <li>firebase</li>
    <li>Django-REST</li>
    <li>Gemini</li>
</ul>

## Usage of tech stack
<p>
We used github for our project workflow, frontend work was started with design choices like colour pallets and the responsiveness of the app. We used figma for designing different pages, it's vector design tools helped us create a wide variety of pages
</p>
<p><b>Django-REST</b> framework was used to create the API for all the communication between the client and the server, it was used for all requests and responses. It was also used to modify the data in a more readable form where it was necessary.
</p>
<p>
The database was initially in the form of json files, to implement searching, <b>gemini</b> was used. First, it was used to map the json files to categories on which we are gonna search upon. Then we used the natural language processing of gemini to map the user prompt of a certain situation into those categories, and return the result with the most weights associated to it.
</p>
<p>
<b>Firebase</b> was used to store the scraped data, and user data, like the user identification and the file system for a particular user. Firebase is used for the OTP verification process, in case a user doesn't have an account, firebase creates one for the user. Firebase provided a seamless interface to apply server side features
</p>
<p>
For the frontend interface <b>flutter</b> framework was used with a wide variety of packages to handle the features that the app offers to users. Some of these packages and their uses were:-
<ul>
    <li><i>file_picker: picking files from external storage</i></li>
    <li><i>flutter_widget_from_html: convert string containing html code to flutter widgets</i></li>
    <li><i>permission_handler: asking user for permissions to manage external storage</i></li>
    <li><i>http: converting files from external storage into a form which can be transferred to firebase</i></li>

</ul>
Flutter was preferred as flutter provides a relatively fast development process and can is easily extensible to multiple platforms like ios and web, which is one of our future targets.
</p>

## Iteration and Challenges
The frontend started with Figma designs and seamlessly transitioned into <b>Flutter</b> development, leveraging its rapid development capabilities for fast paced page creation. During implementation of certain functionalities like external storage file selection, or rendering html strings of legal precedents, we would often encounter the problem of using the right package with the right versions. Flutter goes through upgrades very frequently which makes it hard for a developer to keep up, which also deprecates a lot of online resources even dating a couple of years back. The frontend team often had to refer to the documentation and cross checking the compatibility of packages before using them in the project, this slowed down the process but made the work much more streamlined. 
<p>
A major challenge the team faced was making a file system inside our application, this required collaboration from both the teams working on the frontend and the backend side of the application. Together we figured out a solution in which we store the directory path as a string, and manipulated it whenever a frontend event that changed directories was called, we then shared this variable with the backend to keep track of it so that we don't loose when popping states. 
</p>

The backend team started with the creation of databases with web scraping different websites, it took some time to find the right source that was open to developers. We end up using the [indian kanoon website](https://indiankanoon.org/) for making out database. Then the team proceeded to transfer everything to firebase cloud storage. One of the major challenges encountered by the team was providing the file to the front end interface in the form of an html string to be rendered. Initially, sending the json data byte by byte proved to be a failure, with the reference of some documentation, the team figured out that sending the data through octet streams solved the problem. 

<p>
Some other small challenges faced by the team were tuning the gemini model with the right initialization parameters, it took a lot of experimentation and testing to come up with the right values. Initially, there was a security concerns of the API key being exposed, the team constructed the env file to patch that error.
</p>
