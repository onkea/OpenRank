# OpenRank _Alpha_

OpenRank is a free and open source coding challenges platform, similar to websites like HackerRank, HackerEarth etc. Using this software, individuals solve coding challenges to improve their skills, schools and colleges can host their own coding challenges to evaluate their students and help them learn, corporates and startups can create contests to evaluate and screen potential candidates for job openings before in-person innterviews within their company.

Join the disucssion chatroom for this project on Discord : https://chat.coderplex.org (#open-source channel)

You can view the gist of discussions that happen weekly regarding this project at [Discusionns' gist](/DISCUSSIONS-GIST.md)

This project is still under active development. Code contributions are welcome.

[![Build Status](https://travis-ci.org/coderplex/OpenRank.svg?branch=master)](https://travis-ci.org/coderplex/OpenRank)


## Running :

You can run the apiserver by using the following command

`cd openrank-backend`

`npm install`

`npm run start`

server will be hosted at http://localhost:8000

You can test it by making REST API calls to the URL using curl or postman or any other method of your choice.

To run frontend use the following commands in sequence

`cd openrank-frontend`

`npm install`

`npm run dev`

open http://localhost:3000/ once the server is started

## Unit tests :

You can run the unit tests by running following command in project folder. Make sure you install below mentioned testing module first.

`TODO: Fix on some testing module and update test run command`

## Resources : 
 Next.js 
 - [Getting started with Next.js](https://nextjs.org/learn/basics/getting-started)

 Express.js 
 - [Express.js & Node.js Course for Beginners - Full Tutorial](https://www.youtube.com/watch?v=G8uL0lFFoN0)

Awesome beginners-friendly Projects : https://github.com/MunGell/awesome-for-beginners

## Roles 
The application will have different roles for different users. They are as follows :
- User with "creator" role can :         
  1. Create a new contest
  2. Submit questions with inputs and expected output
- User with "Admin" role can :
  1. See the leaderborad (can also decide whether contestants can view or not)
  2. See all code submissions
- User with "Contestant" role can :
  1. Register and participate in contests
  2. Submit their code, and test for custom inputs


## Tech Stack :
1. Express - Node.js (for backend)
2. Next.js (for frontend)
3. Docker containers (for testing the submitted code)
4. Celery (distributed computing)


### Deadline: Will be updated.

## User Workflow:
- Host on personal server or cloud
- Create a contest:
  1. Provide contest name and other details (Description, Guide, Rules, FAQ, Criteria etc)
  2. Add questions (Challenge name, score, description, sample_input, sample_output, testcases)
  3. Share link generated
- Participate in contest:
  1. Go to link generated for the contest
  2. Register with required details and login
  3. Go through questions and submit code 
  4. Test the code with sample inputs
  5. Test with custom inputs (optional)
  6. Submit for evaluation with all test cases

## Why use this software :
  1. Super easy to deploy to any cloud provider (eg. AWS, AZURE, GCP) or even local servers
  2. It's free. Small companies can use it to conduct coding interviews
  3. Scales really well (automatic evaluataion of code without manual intervention)
