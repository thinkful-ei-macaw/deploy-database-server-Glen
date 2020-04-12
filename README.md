.env file info

NODE_ENV=development
PORT=8080
API_TOKEN="secret-token"

DATABASE_URL="postgresql://dunder_mifflin:123@localhost/noteful"
TEST_DATABASE_URL="postgresql://dunder_mifflin:123@localhost/noteful-test"

To set up Heroku database in the bash prompt

heroku create

heroku addons:create heroku-postgresql:hobby-dev

heroku pg:credentials:url

Use the credentials to set up a dBeaver database


Express Boilerplate!
This is a boilerplate project used for starting new projects!

Set up
Complete the following steps to start a new project (NEW-PROJECT-NAME):

Clone this repository to your local machine git clone BOILERPLATE-URL NEW-PROJECTS-NAME
cd into the cloned repository
Make a fresh start of the git history for this project with rm -rf .git && git init
Install the node dependencies npm install
Move the example Environment file to .env that will be ignored by git and read by the express server mv example.env .env
Edit the contents of the package.json to use NEW-PROJECT-NAME instead of "name": "express-boilerplate",
Scripts
Start the application npm start

Start nodemon for the application npm run dev

Run the tests npm test

Run the linter npm run lint

Run prettier formatting npm run format

Deploying
When your new project is ready for deployment, add a new Heroku application with heroku create. This will make a new git remote called "heroku" and you can then npm run deploy which will push to this remote's master branch.