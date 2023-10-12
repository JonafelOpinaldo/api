Jonafel Opinaldo 4-A
# API Name
API Demo

# Brief Description
This is a simple RESTful API built with PHP and the Slim framework for interacting with a 
MySQL database. It provides endpoints for creating, reading, updating, and deleting records in a database table named "names."
 
## API
Endpoints
**GET /getName/{fname}/{lname}**
**Function:** Retrieve a greeting message that includes a user's first name and last name.
**Required Parameters:** fname (first name), lname (last name).

**POST /postName**
**Function:** Insert a new record with first name and last name into the "names" database table.
**Request Payload:**![image](https://github.com/JonafelOpinaldo/api/assets/147078489/445177a6-3d78-4893-bc4b-576d55e023cf)

**GET /postPrint**
**Function:** Retrieve all records from the "names" database table.
**No required parameters.**

**PUT /updateName/{id}**
**Function:** Update an existing record in the "names" table by providing the record's id.
**Required Parameters:** id (record identifier).
**Request Payload:**![image](https://github.com/JonafelOpinaldo/api/assets/147078489/8d3971a4-e067-4c0c-a27d-fd2604d1c015)

**DELETE /deleteName/{id}**
**Function:** Delete a record from the "names" table by providing the record's id.
**Required Parameters:** id (record identifier).
![image](https://github.com/JonafelOpinaldo/api/assets/147078489/1627e364-fb86-4473-b94c-bea0cba34da6)



Explain the structure of the request payload, including any required or optional fields.
You can use JSON examples to illustrate.

**The API expects JSON payloads for POST and PUT requests with the following structure**
{
    "fname":"jonafel",
    "lname":"opinaldo"
}
**IF succesfull response**
{
    "status": "success",
    "data": null
}
**else**
{
    "status": "error",
    "message": "Error message"
}

**Possiblie status codes encountered during the process
404
200**

## Usage
To use this API, you can send HTTP requests to the defined endpoints using a tool like Postman or 
by implementing HTTP requests in your application.

Provide code
examples or instructions on how to use your API.
**example:**
open POSTMAN then type **localhost/api/public/postPrint** select the method **GET**
**localhost/api/public/ - this is the path where I store the source code for my API**
**The Reponse should be the content of your DATABASE**
 
## License
The code does not include a specific license declaration. 
 


## Contributors
Sinclair Schanne Corpuz


## Contact
Information
gmail: jonafel.opinaldo@student.dmmmsu.edu.ph
