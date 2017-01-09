# 100 Days Of Code - Log

### Day 1: January 3, 2016

**Today's Progress**: Cleaned up some missing routes and pushed all of chesmsbl.org to GitHub

**Thoughts:** I'm happy to get cracking on #100daysofCode to help keep me on track for side projects. I've also rallied a few friends, @soldierforus and @jwsummers. I'm looking forward to collaborating on a future project with them. I'm not happy that I'm throwing together the chesmsbl.org site with an express + pug application, but it has allowed me to move very quickly. Hopefully I can switch it over to react + redux in the next couple of weeks.

**Link(s) to work**

1. [Tonight's Commit](https://github.com/stephengfriend/chesmsbl.org/commit/156ca3d9e5ba11dad68a3b126d7798a3ccb85435)
2. [Chesapeake Men's Senior Baseball Leage](https://www.chesmsbl.org)

### Day 2: January 4, 2016

**Today's Progress**: Fixed 404 route, enabled forced https, updated user model

**Thoughts:** I spent my work day more excited to to work on #100daysofcode projects than on my actual work. That's probably because I was knee deep in Google Sheets, Jira tickets, and GitHub commits. @jwsummers came over for dinner and I spent a solid hour just walking through the express application, explaining it's various parts and how they apply to web application development. I'd like to have him add a some static content, as an exercise in learning.

**Link(s) to work**

1. [Tonight's Commit](https://github.com/stephengfriend/chesmsbl.org/commit/ddd4b458f795f57353670c3586e7d4ebcd46acb9)
2. [Mongoose Docs](http://mongoosejs.com/docs/guide.html)

### Day 3: January 5, 2016

**Today's Progress**: Added CircleCI continuous deployment to herok an integrated auth0 login and signup 

**Thoughts:** I had some spare time before work this morning, in that time I setup [CircleCI](https://circleci.com) continuous deployment to Heroku. I'd like to take it a step further and when a collaborator submits a PR, it would fork a dev environment for them to check their changes out. I spent some cycles converting to sequelize and postgres, since the data for this site will be heavily associated and easier to normalize. Tonight I added [Auth0](https://auth0.com) with a custom login and registration page. I wired it up to passport and can confirm logins and signups work. Tomorrow, I need to add steps for new users to complete their profile. Additionally, I need to wire it up to my database backend and check for existing emails from social signups.

**Link(s) to work**

1. [CircleCI Commit](https://github.com/stephengfriend/chesmsbl.org/commit/d217756fe0ab5ef5ebeb2e7372eab8ddcc0bc7b7)
2. [auth0 Branch](https://github.com/stephengfriend/chesmsbl.org/tree/auth0)

### Day 4: January 6, 2016

**Today's Progress**: Added rollbar 

**Thoughts:** I spent most of my programming time integrating various services. I got a free Auth0 OSS account, giving me access to all of the features of Auth0. I also used my GitHub student developer pack to get a SendGrid account provisioned. I linked Auth0 up to SendGrid. I formatted all of the email templates for email verification, forgot password, etc... I also got Rollbar hooked up for tracking errors within the stack. I'd like to wire it up for deployments, so that I can track the errors per deployment.

**Link(s) to work**

1. [Day 4 Commit](https://github.com/stephengfriend/chesmsbl.org/commit/f7fb35ef45643a3f6a2ab03df6761a46bea125c1)

### Day 5: January 8, 2016

**Today's Progress**: Added user and password login, cleaned up the user profile section, and added crisp.im 

**Thoughts:** Saturday was a waste, due to not feeling well. I spent today doing a bit more work. Trying to get the user authentication finished. Login and register work, but there are a few more thinks to work on. Namely, signing up with a social account needs a special flow to get the email and password identity setup. Then the social account needs to be linked to the db account. I also need to work on a second step for filling out the player profile. Wiring it up the user model needs to be tied to the Auth0 account.

**Link(s) to work**

1. [Tonight's Commit](https://github.com/stephengfriend/chesmsbl.org/commit/a80fa7cf2e5c96affcdf6dc5491ca5cfc3ecf1e8)
