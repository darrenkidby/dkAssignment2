# Assignment 2 - Web API.

Name: Darren Kidby

## Features.

- Login and Sign Out with authentication. 
- Added a new header "authHeader". This header allows us to see whether we are logged in or not. Aswell as give a link to the login page. I placed it in the filtermovies card instead of the root index file.
- Protected routes on the favourites page to stop users that aren't logged in to see.
- I added the proxy code to package.json so my react app was connected to my movie-api.
- I added a now_playing, top_rated and popular api into my tmdb-api. This allows me to see those pages on my site.

## Setup requirements.

- To run my react app, I needed to type npm install into the command prompt in the react app directory. After that I had to type npm satrt to make the react app work.
- To run the movies-api, I needed to have mongo running. So, I went to the mongodb bin folder, pressed cmd and typed mongo into the command prompt. Next, I opened my movie-api folder in my assignment, typed cmd, then in the command prompt, typed npm install. lastly, I typed npm run dev to make my database to work. I also had to make sure the .env file was in the document.

## API Configuration

create an `.env` file.

______________________
NODEENV=development
PORT=8080
HOST=
mongoDB=YourMongoURL
seedDb=true
secret=YourJWTSecret
REACT_APP_TMDB_KEY=<Your-Api-Key>
______________________

## API Design
Give an overview of your web API design, perhaps similar to the following: 

- /api/movies | GET | Gets a list of movies 
- /api/movies/{movieid} | GET | Gets a single movie 
- /api/users | GET | Gets a list of users
- /api/genres | GET | Gets a list of genres
- /api/users?action=authenticate | POST | Gets a token

## Security and Authentication

The favourites page has a protected route because I wanted it so users could't see the favourites until they were logged in.

## Integrating with React App

I used integration in my movies-api to login and signup into the react app. It was needed to be able to authenticate the login and signup.

## Independent learning (if relevant)

I added new layout colours to my react app. This works using the css.