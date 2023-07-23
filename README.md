# Simple HTTP Server with CRUD Operations :computer:

This repository contains a simple HTTP server implemented in Node.js using the http module. The server provides basic low level API operations by using request and response streams for managing a list of friends. Additionally, it handles a route to display messages :speech_balloon:

## Usage :rocket:

To start the server, run the following command:

`node index.js`

The server will start listening on port 3000. You can change the port by modifying the `PORT` constant in the `server.js` file.

## API Endpoints :link:

### 1. GET /friends :busts_in_silhouette:

Retrieves a list of friends in JSON format. Each friend object contains an `id` and a `name`.

Example Response:

```json
[
  {
    "id": 0,
    "name": "Nikola Tesla"
  },
  {
    "id": 1,
    "name": "Sir Isaac Newton"
  },
  {
    "id": 3,
    "name": "Albert Einstein"
  }
]
```

### 2. GET /friends/:id :bust_in_silhouette:

Retrieves the friend with the specified id in JSON format.

Example Response:

```json
{
  "id": 1,
  "name": "Sir Isaac Newton"
}
```

### 3. POST /friends :heavy_plus_sign:

Adds a new friend to the list. The friend details should be provided in the request body as a JSON object containing id and name fields.

Example Request:

```
POST /friends
Content-Type: application/json

{
"id": 4,
"name": "Marie Curie"
}
```

### License :scroll:

This project is licensed under the MIT License. Feel free to use, modify, and distribute the code as per the terms of the license. :tada:
