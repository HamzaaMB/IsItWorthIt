# Is It Worth It? - GA Project Two

## Brief

Second project for the Software Engineering Immersive course, a React app pair-coded with GA classmate Patrick Johnson in a 48-hour hackathon.

## Deployment

App has been deployed with Netlify can be viewed here: [Is It Worth It?](https://isitworthit-hb.netlify.app/)

## Technologies Used

* React.js
* JavaScript (ES6)
* HTML5
* SCSS
* Axios
* React Router Dom

### API
* restcountries.eu
* travelbriefing.org

### Dev tools

* VS Code
* Insomnia
* Yarn
* Git
* GitHub
* Figma (Wireframing)
* Netlify (Deployment)

## Overview and Concept

After fighting the temptation to use the Rick and Morty API, we concluded that creating an app designed to help users in picking their holiday destination would seem perfect. Given the current climate of the world, we wanted to include all the information provided to us by APIs about all the countries which would make it easier for our users to make their decision.

![screenshot](IsItWorthIt/screenshots/homepage.png)

## Approach Taken

### Planning

Due to the deadline of 48 hours, our first task at hand was to find public APIs that would provide sufficient data for us to be able to use. Since we weren’t able to find one, we decided to use two APIs that would compliment the other. Once we found the API’s, we wireframed our components and what they would look like. Google docs in particular helped, as me and my teammate threw all the ideas we could think of on there and then trimmed it down to sections, MVP and Nice-To-Haves.

![screenshot](IsItWorthIt/screenshots/googledoc.png)

## Process

Our process first included testing the API’s we had chosen extensively, to figure out what the data structure looks like. As we were using public API’s, we had to get familiar with different endpoints, what data they represent and which one we actually need for our app. Being particularly new to Insomnia and Axios, we managed to load them up on the browser in the form of logs to make sure all the data we needed was coming through. 

![screenshot](IsItWorthIt/screenshots/insomnia.png)

The component that showed all our countries used the endpoint shown above, in the form of a GET request. 

![screenshot](IsItWorthIt/screenshots/countryindex.png)

Next step was to create a component that shows the information of each individual country, based on what the user clicks. For this we had to keep a few things in mind, first was to create a new route for the country show page.

![screenshot](IsItWorthIt/screenshots/path.png)

In the component of country show, we created a get request for the second API, which worked in our case as across both APIs the country names were consistent. 

Based on what the user chooses, we had Params in place that would make a request for data attached to that specific country. We were then able to add all this data and render it on the page along with a drop-down for average temperatures across the year. 

![screenshot](IsItWorthIt/screenshots/getrequest.png)

The drop-down for the weather was attached to a conditional render, that would popup with a message based on which month the user selected.

![screenshot](IsItWorthIt/screenshots/dropdown.png)
![screenshot](IsItWorthIt/screenshots/countryshow.png)

## Bugs and Blockers

* We faced CORS for the first time and learnt how to tackle it, it was by far the biggest challenge we had faced. We were able to add cors-anywhere.herokuapp.com, at the beginning of the URL for our request made, which gave us enough time on this project to finish off our testing phase.

* As we weren’t able to make that many requests to the API, we had to find other ways of working on the app without reloading the page. Chrome Dev Tools really came in handy and we did all of our styling in the browser.

* The biggest bug we have is that restcountries.eu API has more countries than travelbriefing.org. Which means that some of the countries on the ‘all countries’ page do not link to the ‘show country’, which in result just shows you the nearest country to the alphabet you have clicked as a user.


## Wins

* We reached MVP and were also able to add the search filter - that being part of our Nice-To-Have.
* First time working with APIs and learning more about requests at this stage, I feel this project, although was 48 hours, elevated me to have a much better understanding. 

## Future Content & Improvements

* Only show countries which both APIs have in common to avoid the bug
* Create a more interactive page for country show with additional information
* Error handling
* Add more styling to the project overall

## Key Learnings

This project was my first attempt at creating requests and using APIs, which served me well. Also the first time I paired up with someone to code, which was also an amazing experience, really learnt how to tackle problems and work together. 



