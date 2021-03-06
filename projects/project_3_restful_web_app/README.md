# RESTful web api - private blockchain

A RESTful blockchain webapp that adds new block to blockchain and also let you see the blocks at a particular blockheight

## Architecture
Local Server
- Node.js
- Express.js

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

Installing Node and NPM is pretty straightforward using the installer package available from the (Node.js® web site)[https://nodejs.org/en/].

### Configuring your project
- Clone/Download the project and cd into the root folder
- Install all dependencies via npm.
```
npm install
```

## Running project
- Create `.env` file in root of the project which will have our custom node env vars
```
# Sample .env file
PORT = 8000
NODE_ENV = development
```

- Run command
```
npm start
```
and now open `localhost:<PORT>` in your browser window.

## Endpoints

### GET endpoint
**Fetch block at a particular blockheight**
```
http://localhost:<PORT>/block/blockheight
```

### POST endpoint

**Add new block**
```
http://localhost:<PORT>/block
```
**Params**
```
{
  "body": "This is body text for block!"
}
```
