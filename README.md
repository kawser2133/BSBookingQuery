# BSBookingQuery

Hotel Booking System
This is a backend application for a hotel booking system. It allows users to search for hotels, leave comments, and make bookings.

Getting Started
Prerequisites
.NET Core SDK 3.1 or higher
Microsoft SQL Server 2012 or higher
Installing
Clone the repository to your local machine.
Open the solution file in Visual Studio or your preferred IDE.
Update the connection string in the appsettings.json file to point to your SQL Server instance.
Open the Package Manager Console and run the following command to create the database:
sql
Copy code
Update-Database
Build the solution to restore NuGet packages.
Running the Tests
The unit tests can be run from the Test Explorer in Visual Studio or by running the following command in the Package Manager Console:

bash
Copy code
dotnet test
Usage
Hotels
Get All Hotels
bash
Copy code
GET /api/hotels
Returns a list of all hotels.

Get Hotel by Id
bash
Copy code
GET /api/hotels/{id}
Returns a specific hotel by ID.

Get Hotels by Name
bash
Copy code
GET /api/hotels?name={name}
Returns a list of hotels matching the specified name.

Get Hotels by Location
bash
Copy code
GET /api/hotels?location={location}
Returns a list of hotels in the specified location.

Get Hotels by Rating Range
bash
Copy code
GET /api/hotels?minRating={minRating}&maxRating={maxRating}
Returns a list of hotels with ratings in the specified range.

Add Hotel
bash
Copy code
POST /api/hotels
Adds a new hotel.

Update Hotel
bash
Copy code
PUT /api/hotels/{id}
Updates an existing hotel.

Delete Hotel
bash
Copy code
DELETE /api/hotels/{id}
Deletes an existing hotel.

Comments
Get Comments by Hotel Id
bash
Copy code
GET /api/hotels/{id}/comments
Returns a list of comments for the specified hotel.

Add Comment
bash
Copy code
POST /api/hotels/{id}/comments
Adds a new comment to the specified hotel.

Reply to Comment
bash
Copy code
POST /api/comments/{id}/replies
Adds a new reply to an existing comment.

Users
Get All Users
bash
Copy code
GET /api/users
Returns a list of all users.

Get User by Id
bash
Copy code
GET /api/users/{id}
Returns a specific user by ID.

Add User
bash
Copy code
POST /api/users
Adds a new user.

Update User
bash
Copy code
PUT /api/users/{id}
Updates an existing user.

Delete User
bash
Copy code
DELETE /api/users/{id}
Deletes an existing user.

Built With
.NET Core 3.1
Entity Framework Core
AutoMapper
Serilog
