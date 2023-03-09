# Hotel Booking System

This is a backend application for a hotel booking system. It allows users to search for hotels and leave comments.

## Prerequisites

* .NET Core SDK 3.1 or higher
* Microsoft SQL Server 2012 or higher

## Installing

1. Clone the repository to your local machine.
2. Open the solution file in Visual Studio.
3. Update the connection string in the appsettings.json file to point to your SQL Server instance.
4. Open the Package Manager Console and run the following command to create the database:

```bash
Update-Database
```
5. Build the solution to restore NuGet packages.

## Usage
#### Hotels
* /api/Hotel/get-by-id/{id}
* /api/Hotel/get-all
* /api/Hotel/get-by-name/name/{name}
* /api/Hotel/get-by-location/location/{location}
* /api/Hotel/get-by-rating/rating/{minRating}/{maxRating}
* /api/Hotel/create
* /api/Hotel/update/{id}
* /api/Hotel/delete/{id}

#### Comments
* /api/Comment/get-all
* /api/Comment/get-by-hotelid/hotel/{hotelId}
* /api/Comment/add/hotel/{hotelId}
* /api/Comment/reply/comment/{commentId}
* /api/Comment/update/{id}
* /api/Comment/delete/{id}



## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License

[MIT](https://choosealicense.com/licenses/mit/)
