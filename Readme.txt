﻿Author name: Arpan Arpan
date: october2,2023
Hi there I am working with the ASP.NET Core 3.1 and making an application called MvcMovie.

Oh God my browser doesn'nt worked.
So I go to launchsettings and commented the sslport, and now it works.

I changed my index page with Hello World instead of Welcome.

PART2:

In second i need to add the controler, So here i go and add the controller.I added the MVC Controller under the controller;s folder and named it HelloWorld Controller.
I replaced the content of the HelloWorld.cs file as provided in the tutorial.
Yeah......!! It prints my message of the actions.

Later on i updated the welcome method to two different parameters, to pass some information to the url.
I checked and pass the parametre in URL , Damn!!! It worked.
 Lets change some more , i tried with ID parameter instead of numtimes and i am gonna check what will happen!!
 Yes it printed my value when I pass the parameter"https://localhost:{PORT}/HelloWorld/Welcome/3?name=Rick"
 With this I completed my PART 2 of the tutorial.

 PART3:
 So I started the part three which is all about View. 
 So in my first step I added an HelloWorld folder in my View folder. Later on i added an index.html file in it. This gonna show my HelloWorld method's Index page.
 I change the code with the provided code in the tutorial. 
 Also I changed my HelloWorld.cs file in which I surpass the return View() functiojn , So that I can see that index page I have created.
 Guess what it said it hass build in errors, So I found out that the Index method pass the string value so I changed it to IActionResult, then my App runs smoothly.

 Now I created a ViewData dictionaly for welcome and passes the numTime and name parameteres in it. This will pass my parameters to the View directly.
 Now I created a Welcome.html file under the View/HelloWorld folder.I will create a loop in it which will show the hello+ numtimes value in it. Now I can print my name the number of times which number i'll assign to the numtimes.
 Since i typed the "https://localhost:{PORT}/HelloWorld/Welcome/?name=Arpan&numTimes=8" It printed Hello Arpan 8 times.
 I will surely say Yeah It worked!!!!!!!!!!
 And my PART 3 is complete.

 PART4:

 Let's Go for the part 4

 Here I an working on the Models .
 In my Models folder , Added the Class in it with the name Movie.cs
 When i tried to install the package it pop up with the error says that its installed version 7 is not compatible . So i went to the tools and 
 in in manage nuget packages i installed the latest version of 3.1 for it. Now its good to go.
 Moving forward with the next part I added the Data folder in the MvcMovie and add a controller named MvcMovieContext.cs file in it. 
 I changed the code of the file according to the provided code in the tutorial and we are good to go for next now .

 Since I have created the database I need to register it. So as per instructions , I updated my startup.cs file with the given code:
 "using MvcMovie.Data;
   using Microsoft.EntityFrameworkCore;". Later on I also updated the startup configureservices.
   Now lets see If it works or not.

   Everything it done related to the database, We created it, registered it . Now we have to examine our database. So I changed my appsettings.json file and added the code given in the tutorial.

   Next step was to add a scafollding item  to create the movie pages(CRUD) for the movie model.
   The step was to , to add a scaffolding item in the Controller folder.
   When I created it it pops up the error says the Entity framework doesn't exist.
   But that not a big deal because it needed a initial create which i have;nt done.
   So I run the command
   "Add-Migration InitialCreate"
   "Update-Database"
   And guess what my Migrations folder created out. That was easy now we are safe...........!!!!


   My MvcMovie link was not working and it was showing the database. So I figured out that my scafollding was not dpone properly
   So I again repeated the procedure of adding scaffolding item and now it works.......!!!!
   Thank God
  
  PART 5:

  Adding the data of the movies.
  It was not that hard the instructions was to create a class under the Model folder and name it SeedData.cs and I did the same. Now what replaced the code with the given entries of the movies.
  I updated the program.cs file to run the seedData. 
  After that I run the application and guess what it din'nt worked.
  It is a trouble, then I remembered that I added the data in the file but what about the update. I should update it so thatdatabase came to know there is a change of data in it. 
  Then i Updated it and it worked I can clearly see my Movies information that has been added.



  Part6:

  Adding a search string method, which will search the movie for me.
  I got an error which is "searchString doesn not exist in the current context". I can'nt figure it out yet , but we will be working on it.