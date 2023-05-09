# MongoDB CRUD Operations with Express.js

This is a practice project for performing CRUD (Create, Read, Update, Delete) operations on a MongoDB database using Express.js.

## Prerequisites
- Node.js <br>
- Express.js <br>
- MongoDB

## Dependencies
This project uses the following dependencies:
* express
* mongodb
* nodemon

## Usage
1. Clone the repository
2. Install dependencies using npm install
3. Start the MongoDB server on your local machine.
4. Use a REST client (such as Postman) to test the CRUD operations.

## Database Connection
The database connection is established using the MongoClient from the mongodb package. The connectToDb function in db.js is used to connect to the database and the getDb function is used to get the database instance.

## API Endpoints
* GET **/books** <br>
  Returns all books in the database sorted by author name in ascending order.

* GET **/books/:id** <br>
  Returns a book with the specified ID.

* POST **/books** <br>
  Creates a new book in the database. The request body should contain a JSON object with the following properties:  <br>
     - name (string): The title of the book <br>
     - author (string): The author of the book <br>
     - pages (number): The pages in the book <br>
     - price (number): The price of the book <br>
 
 * PATCH **/books/:id** <br>
  Updates a book with the specified ID. The request body should contain a JSON object with the properties to update.

* DELETE **/books/:id** <br>
  Deletes a book with the specified ID.

## Contributing
If you would like to contribute to this project, please fork the repository and submit a pull request.

## License
This project is licensed under the MIT License. See the LICENSE file for details.
