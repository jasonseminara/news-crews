
# News Crews (name not final)

The News Crews app is for consumers who enjoy good conversation while digesting their daily dose of news. 

Here at News Crews, we want to make news more social. How you might ask? Once you're a registered user (it's super simple) you can curate or join groups with similar interests to you. As a group admin, you can choose to invite users or go public, allowing users to join themselves without permission. Within your group, each user will receive five articles per day (derived from their favorite topics) and can select only one to discuss with the group. Thats it!

Have fun, start reading and never stop discussing!

## User Stories Idea 2 (social news app):
- As a user of ... I want to read news articles online
- As a user of ... I want to stay in-touch with friends through the discussion of current events
- As a user of ... I want exposure to news articles I wouldn't typically read via discussion group votes
- As a user of ... I want to save and share my favorite news articles with friends and for personal browing later
- As a user of ... I want to join random groups for article discussion

## ERD:
1. Table Users: id(spk), Username, Password, F_Name, L_Name, Email, Created_At
2. Table Groups: id(spk), Description, Created_At, Creator (REF Users.id)
3. Table Comments: id(spk), Author(REF Users.id), Content, Created_At, Group_id(REF Groups.id)
4. Table Articles: id(spk), URL, Source, Created_At
### M:M 
5. Table User_Groups: id(spk), User_id(REF Users.id), Group_id(REF Groups.id)
6. Table Group_Articles: id(spk), Group_id(REF Groups.id), Article_id(REF Articles.id)

![img_20180801_134100](https://media.git.generalassemb.ly/user/14895/files/2a94cb4e-9593-11e8-85e7-57aa0be8387e)

## Wireframe:

This is a very rough sketch but I will be using Bulma to style this project. More views will come into play as the project concept matures:

![img_20180801_134624](https://media.git.generalassemb.ly/user/14895/files/5d13bdd2-9593-11e8-9599-a0d3344ec694)

## Flowchart:

![screen shot 2018-08-03 at 9 57 04 am](https://user-images.githubusercontent.com/34017019/43646710-a266a806-9703-11e8-8f31-35e723162023.png)

## Project Resources & Shoutouts:

### People:
1. @John Master - Thank you for all the awesome auth functions.
2. @Jason Seminara - Thank you for all the help with route discussion and controller functions.

### npm packages:
1. bcryptjs v: 2.4.3
2. body-parser v: 1.18.3
3. bulma v: 0.7.1
4. connect-flash v: 0.1.1
5. dotenv v: 6.0.0
6. ejs v: 2.6.1
7. express v: 4.16.3
8. express-session v: 1.15.6
9. method-override v: 3.0.0
10. morgan v: 1.9.0
11. node-fetch v: 2.2.0
12. passport v: 0.4.0
13. passport-local v: 1.0.0
14. pg-promise v: 8.4.5
15. eslint v: 4.19.1 AIRBNB STYLEGUIDE
16. nodemon v: 1.18.3



