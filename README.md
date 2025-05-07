# golang-crud
Simple CRUD made with Golang to learn the language. Project made following HunCoding playlist on YT.

## Step by step of what I did 

### Creating main.go and initiating go.mod file

First I runned the command `go mod init github.com/isnotvinicius/<project-name>` to create the `go.mod` file.

Then I created the `main.go` and `.env` files on the root of the project. After creating the `.env` file, I've imported the `godotenv` library to be able to use the `.env` variables in my project

### Setting up the folder structure

In order to organize the code, I created the `/src` folder in the root of the project which will contain all the MVC structure of the project along with the test and configuration modules.

### Error handling

Inside the `configuration` package, I created the `rest_err` package and it's file to handle all the errors of the API. Then I created some structures to deal with the errors on the API.

After creating the base structures, I created some functions to deal with multiple types of errors using the created structures. 

And to finish it, I created the `Error()` function to be able to log all errors in the API.

### Creating the Routes and first controllers

To manage the routing of the API, I've used the `Gin Gonic` library to deal with the requests.

After installing `Gin Gonic`, I've created the `routes` package inside `/src/controller` and inside it I added all the routes I'll need for the API to run.

Then I created one controller file for each of the CRUD words.
