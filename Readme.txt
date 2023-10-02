Author name: Arpan Arpan
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
 in in manage nuget packages i installed the latest version of 3.1 for it. Now its good to go