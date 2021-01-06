# FotoFab
Foto Fab
Using Unsplash Api
─
Name:
Shivam Yadav
Front-End Project
1
Table of content:
1.Introduction
2.Pages
3.Components
4.Api Endpoints
5.Key Features
6. Extra Features
7. Technologies Used
8.Issues Faced
9. Future Aspects
2
Introduction
The web App is made with React and is dedicated to sharing stock photography.Beautiful, free
photos are shared by the world’s most generous community of photographers.
It grants an irrevocable, nonexclusive, worldwide copyright license to download, copy, modify,
distribute, perform, and use photos from Unsplash for free, including for commercial purposes,
without permission from or attributing the photographer,Unsplash or the Foto Fab web app.
Pages
Login
The login page guides the user to login with a Unsplash account which is essential to access
the profile page of the user which contains features such as the photos uploaded by the
user,photos liked by the user and his personal collection of photos.
Homepage
The homepage comprises of a navbar ,searchbar and a photo section which contains a list
of endless photos provided by unsplash.The navbar has a logo of Fotofab which is linked to
the foto fab homepage.It also has a home button followed by a login or a logout button
depending on the state of the web app.In case the user logs in with the unsplash account a
profile picture of the user will be visible on the navbar followed by the logout button.
The search bar has a random image present in the background which is fetched from the
api as well.The search bar leads the user to a search page which contains the photos of the
requested item.The keyword used for the search could be of a user or a collection as well.
When the images are hovered ,a download button pops up which can be used to download
the image.The other thing that pops up is the profile of the image owner as well as a like
and add to collection button.The profile name can be used to land on a profile page of the
photographers.The like button will add the current photo to a list of liked photos of the
user currently logged in.The add to collection button button will guide the user to add the
photo to an existing collection.
3
The top right corner has a sticky bar which contains the social links to the pages as well as
links to about page and contact page as well.
Detail Page
The detail page has a profile picture of the photographer on the top left corner followed by
the name provided by the profile owner along with the location and the social links.By
clicking on the location the user can get a detailed map view of the location while the social
link will lead the user to their social pages.A little description is also provided right next to
it. The top right corner has download button which drops down into four more buttons via
large,small,medium and original.The user can download the photos based on its choice.The
middle section has a preview of the image that has been clicked.The image is followed by
the tags which will lead the user to their specific search pages.After that there’s a section
containing the caption followed by a statistics section which shows a count of total
likes,views and downloads.Then comes a section that holds the detail regarding the focal
length ,the device used etc and finally there’s a collection section which shows results of the
related collection.
Search Page
The search page consists of photos related to the searched keyword.A bar displaying the
searched word.The user gets three options along with the search i.e search
photos,collection or the user.Each of these options lead the user to their desired pages.
User Profile Page
The user profile page has the profile picture of the user followed by the name and the
bio.Right next to it is the edit profile button which leads the user to a edit profile page
which has three input fields first name,last name and bio.As soon as the user changes the
input fields and presses the save button the user profile details get updated or the user can
press the cancel button to discard the changes.
The user profile page also has a photo tab which contains all the photos uploaded by the
user on the unsplash.Then comes the like part which contains the pictures liked by the user
and the last one is the collection which shows the user collection.
Edit Profile Page
4
The edit profile page which has three input fields first name,last name and bio.As soon as
the user changes the input fields and presses the save button the user profile details get
updated or the user can press the cancel button to discard the changes.
Collection Page
Whenever a user clicks on the collection ,it leads the user to a new page which is the
Collection page.The topmost bright colored gradient bar depicts the name of the collection
Followed by the images present inside the collection.
About us Page
The about us page reveals the name and the images of the developers.This page can be
used to describe the company goals and future aspects as well.
Contact us Page
The contact us page can be accessed by clicking on the contact button present in the
floating social icons bar.The contact page has three input fields title,email and content
followed by a send mail button.This page can be used by the user to send mails to the
foto-fab developers.
Components
I. Alert model
This component is specifically built to handle all the alerts instead of using the
inbuilt browser alert.
II. About photo
This component contains the animations displayed on the about us page.
III. Collection
5
This component is used to display the pictures in the card structure
IV. Mobile Navigation
This component displays a bottom div which has a home button and the profile
picture of the user currently logged in when the screen width reaches a threshold of
800px.
V. Modal
This component is used to display the location which is the google map in a modal
like structure.
VI. Navbar
This component is used to hold the logo ,nav links,buttons and the profile picture of
the user logged in.
VII. Photo card
This component holds the image fetched from the api which is displayed in the form
of a card like structure.
VIII. Protected route
This component ensures that only logged in users can access certain parts of our
site that may contain private user information.
IX. Public User collection
This component provides a structure to the images present inside the collection.
6
X. Public User likes
This component provides a structure to the images present inside the like section
of the public user.
XI. Public User photos
This component provides a structure to the images present inside the photos
section of the public user.
XII. Search bar
This component has the input field which takes the keyword from the user as an
input.
XIII. Searched Collection
This component displays the collection structure once the user searches for a
collection.
XIV. Searched photos
This component displays the structure once the user searched images for a specific
keyword.
XV. Searched User
This component displays the pictures of the users in a card form once the user
searches using the username.
XVI. Search form
This component displays a random image fetched from the API along with the
name.
7
XVII. Spinner
This component is used to display an animated spinner while the data is being
fetched.
XVIII. Sticky Bar
This component displays floating sticky social icon handles and a few pages on the
right corner of the screen.
XIX. User Profile
This component displays the profile picture,name and location at the top of the
profile page.
XX. View Profile
This component was used to display the profile picture of the user that was clicked
on.
API Endpoints
Two APIs are used in this project
1. MAPQUEST
2. UNSPLASH
The endpoints of Mapquest are
1. Base Url/geocoding/v1/address?key=KEY&location=Location
The endpoints of Unsplash are
1. Public Authentication:
GET/photos/?client_id=YOUR_ACCESS_KEY
2. User Authentication:
8
GET/oauth/authorize
3. GetCurrent user profile:
GET/users/auth
4. Edit current user profile:
PUT /me
5. Get public user profile:
GET /users/:username
6. Get public user portfolio Link:
GET /users/:username/portfolio
7. List a users’ photos:
GET /users/:username/photos
8. List a users’ liked photos:
GET /users/:username/likes
9. List a users’ collection photos:
GET /users/:username/collections
10. Get a photo statistics
GET /photos/:id/statistics
11. List photos
GET/photos?page=page-no
9
12. Get a photo
GET/photos/:id
13. Get a random photo
GET/photos/random
14. Like a photo
POST /photos/:id/like
15. Unlike a photo
DELETE /photos/:id/like
16. Search photos
GET /search/photos
17. Search user
GET/search/users
18. Search Collection
GET/search/collections
19. Get a collection
GET/collections/:id
20. Get a related collection
GET/collections/:id/related
21. Create a new collection
POST/collections
10
22. Add a photo to a collection
POST/collections/:collection_id/add
Key features
The Infinite scroll served as a key feature of the entire project.As soon as the scroll bar
reaches the bottom of the screen, a new set of images are fetched which gives a never
ending pool of images.It is used in probably every page.
Extra features
The Geo location serves as an extra feature to the user profile page. By clicking on the
location link ,a user can enjoy the view of a real time google map.The mapQuest api is used
to convert the data in the form of latitudes and longitudes.(Forward Geocode) and then this
latitude and longitude is entered as a parameter in the google-map-react.
Technologies Used
1. axios": "^0.19.2"
2. font-awesome": "^4.7.0",
3. "google-map-react": "^2.0.8",
4. "node-sass": "^4.14.1",
5. "react-redux": "^7.2.1",
6. "react-router-dom": "^5.2.0",
7. "react-spring": "^8.0.27",
11
8. "react-scripts": "3.4.1",
9."redux": "^4.0.5",
10. "redux-devtools-extension": "^2.13.8",
11. "redux-thunk": "^2.3.0"
12. "enzyme": "^3.11.0"
13. “Heroku”
14. “Figma”
Issues Faced during the project
After deploying the project on heroku ,the photos in the collection section are not visible in
chrome but they are visible on safari and microsoft edge.
The create collection takes a lot of time to update the collection.
Future Aspects
A lot of work can be done on the remaining end points like update a collection ,delete a
collection,update photo etc.
