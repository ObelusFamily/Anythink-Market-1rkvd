# Anythink Frontend

The Anythink Frontend is an SPA written with [React](https://reactjs.org/) and [Redux](https://redux.js.org/)

## Getting started

Setup your frontend and backend

1.) Install docker, then verify that it is installed properly docker -v and docker-compose -v
2.) Clone the following repo: https://github.com/ObelusFamily/Anythink-Market-1rkvd.git
3.) Navigate to "Anythink-Market-1rkvd" directory
4.) Run "docker-compose up" 
5.) If docker is setup properly then you will be able to create a new user "http://localhost:3001/register"

What if docker isn't working?
1. Make sure that you have downloaded the latet version, or update the version you are using. 
   Instructions on how to do both can be found here -> https://www.docker.com/

Make sure your server is up and running to serve requests.

## Pages overview

- Home page (URL: /#/ )
  - List of tags
  - List of items pulled from either Feed, Global, or by Tag
  - Pagination for list of items
- Sign in/Sign up pages (URL: /#/login, /#/register )
  - Use JWT (store the token in localStorage)
- Settings page (URL: /#/settings )
- Editor page to create/edit articles (URL: /#/editor, /#/editor/slug )
- Item page (URL: /#/item/slug )
  - Delete item button (only shown to item's author)
  - Render markdown from server client side
  - Comments section at bottom of page
  - Delete comment button (only shown to comment's author)
- Profile page (URL: /#/@username, /#/@username/favorites )
  - Show basic user info
  - List of items populated from seller's items or user favorite items
