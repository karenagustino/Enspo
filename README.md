# Enspo

## Inspiration 
In order to create our solution for this hackathon prompt, we looked into understanding the business model of Aritzia. Their mission is everyday luxury, so we decided to create of a lookbook generator: Enspo.

## What it does 
Users can click on a piece of clothing they like on the Aritzia website, and are led to an extension with a lookbook of similar styles that would go well with their choice. This gives users the ability to customize their wishlists and create a personal shopping experience. Each board displays an aesthetic depending on keywords such as “cozy” and “athletic." There will be functionality to regenerate a new aesthetic board numerous times with the same piece of clothing, as well as an option to save to their lookbook.

## How we built it 
The webpage was built using React, HTML, CSS and the backend architecture used a separate hosted ExpressJS server and NodeJS. A dataset of 40 Aritzia clothing articles was entered in a JSON format. The clothing articles contain 5 fields, the id, link, imglink, sale, tags. The backend will take a keyword from the main clothing article and loop through the tags in the JSON file, sending an API request for the AI through a separate backend server using Axios to generate an average value that indicates how close the clothing article matches. The lookbook will then be generated based on those values.

## Challenges we ran into 
Since we worked on the UI and backend separately, we ran into conflicts merging our branches into our main. There were also issues with connecting the front and back end, as we tried to host it purely on one server. We also had to come up with a way of associating the tags to the keyword which was solved with the API.

## Accomplishments that we're proud of 
We used OpenAI as an API for the backend to solve the problem of generating the lookbook.

## What we learned 
Using React, parsing JSON files in React, API connection, coding in javascript and NodeJS. We also learned about Aritzia's business model.

## What's next for Enspo 
Improve people’s shopping experiences through providing inspiration and recommendations based on their interests. We hope this allows them to venture out of their comfort zone through an array of different products they are introduced to through our application. We would also add a banner for sale items, and expand the number of boards available in a lookbook.
