# Pierre's Treats

## USE

A web page that lets users create an account, add and store treats/flavors. App can keep track of multiple treats with multiple flavors. 

## SET-UP

- Clone the repository
- Navigate to project directory and run the command "dotnet restore" in the terminal, then run "dotnet ef database update"
- Launch the server by running the command "dotnet watch run" and follow the route to use the application.


## SPECS

The application should have user authentication and a user should be able to log in and log out. Only logged in users should have the create, read, update, and delete functionality. Otherwise, the user should be allowed to read-only.
There should be a many-to-many relationship between Treats and Flavors. A treat can have multiple flavors and a flavor can be found in multiple treats. For instance, the "salty" flavor could include caramel and sea-salt ice cream.
A user should be able to use a splash page that lists all treats and flavors. Users should be able to click on an individual treat or flavor to see all the treats/flavors that belong to it.

| Behavior | Input | Output |
|-|-|-|
| user should be able to create an account | 'create account' | _navigates to register page_ |
| user should be able to register| 'username: xxxxx@xxxx.com password: xxxxx' | _creates username with password and stores in database_ |
| user should be able to log in | 'username: xxxxx@xxxx.com, password: xxxxx' | _authenticates user, redirects to account index_ |
| user should be able to log out | 'log out' | _logs user out, redirect to account index_ |
| user needs account to be authorized to create, update and delete | 'create new treat' | _checks user authorization to create a new treat_ |
| user should be able to add treats | 'Caramel' | _adds 'Caramel' to treats table_ |
| user should be able to add flavors | 'Sweet' | _adds 'Caramel' to flavors table_|
| user should be able to add a flavor to a treat | 'Add Sweet to Caramel' | _updates relationship between treat and flavor for those items_ |
| user should be able to add many flavors to a treat | 'Add Salty to Caramel' | _updates relationship between treat and flavor for those items_ | 

## TECHNOLOGIES

C#, cshtml, MySQL, EntityFramework, VS Code;

## AUTHOR

Brendon Tse
brendonjtse@gmail.com

## LICENSE

Open source (2019)