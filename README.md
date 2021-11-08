# Project1

Created Project to Deploy ASP.NET Core MVC App using VS Code and deployed using Webapp service

Steps:

1. Install C# extention in VS Code 
2. Create a folder mkdir Project1
3. Add a solution file to the folder - dotnet new sln
4. create MVC project using - dotnet new mvc -n mvc-web-app
5. Add the project to the solution - dotnet sln add ./(path to .csproj)
6. Open the solution folder in VS Code and open file - when prompted toadd build files click yes. This adds a .vscode folder to solution and creates launch.json and task.json files.
7. Now we have a MVC application that we can run and debug. Use Run menu to start Debugging and webpage will be launched in localhost.

**Services**

1. From the solution folder add a class library using - dotnet new classlib -n Services
2. Add the services project to solution - dotnet sln add Services/Services.csproj reference lib/lib.csproj

It is then possible to create interface and services and hook them up using dependency injection in the usual way.

**UNIT TESTING**

1. From the solution folder add an xUnit test project - dotnet new xunit -n UnitTests

2. Add the Test project  to the solution -dotnet sln add UnitTests/UnitTest.csproj
3. Add a reference to the Service Project -  dotnet add UnitTest/UnitTest.csproj reference Services/Services.csproj
4. Write a xUnit test that tests a service call
5. run the test by using dotnet test in terminal window.



Source Control

1. Create a git repo, add ., commit and push code to Repo

