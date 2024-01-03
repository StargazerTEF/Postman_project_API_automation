# Postman_project_API_automation
### IT Bootcamp final API project

This is a project for API automated testing using Postman and Newman.

### Getting started

- Download zipped [API project](https://github.com/davellanedam/node-express-mongodb-jwt-rest-api-skeleton)
- Unpack the zipped file
- In the extracted folder you will find a file `.env.example`
- Create a new file by copying and pasting the file and then renaming it to `.env`
- Open terminal from the project folder and run following commands respectively: `npm install`, `npm run fresh` and `npm run dev` to run a server.
- Server will be started with url `http://localhost:3000` which is a base url for the project

### Dependencies used
- Node.js
- Postman
- Newman

### API features

- Custom email/password user system with basic security
- HTTP request logger in development mode
- User roles
- User profile
- Users list for admin area
- Cities model
- Testing with mocha/chai for API endpoints
- Ability to refresh token
- JWT Tokens, make requests with a token after login with Authorization header with value Bearer yourToken where yourToken is the signed and encrypted token given in the response from the login process

#### Tests are categorized in the following groups:
- Authorization tests: API requests for login, registration, verification, password reset and refreshing tokens
- City tests: API requests for cities data, filtering, creating new cities, editing and deleting created cities
- Profile tests: API requests for registering profile, login, getting profile information, editing profile and changing password
- User tests: API requests for creating users, login, filtering results, editing data and deleting created users

### Running the tests

#### Postman documentation for this project can be found [here](https://documenter.getpostman.com/view/30403924/2s9YsFFEde).
- For running API requests in Postman after running the server and visiting test documentation link, click on 'Run in Postman' button, create a fork and import a collection.
- To run a collection from the command line using the URL, use a command `newman run https://api.postman.com/collections/{{collectionId}}?apikey={{API key}}`.
- Alternatively you can run the collection from an exported file, by using a command `newman run "exported_file_name.postman_collection"`
