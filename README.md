# alx-project-0x14  

# API Overview  

```
## Available Endpoints

/search: Allows you to search for movies, TV shows, or actors by name.

/movie/{id}: Fetch detailed information about a specific movie by its ID.

/trending: Retrieve a list of trending movies or shows.

/genre/list: Get a list of all available genres.
```

## Request and Response Format  

Request Format

Requests are typically sent using HTTP GET or POST methods. For example:
```
GET https://api.moviesdatabase.com/v1/movie/{id}
Headers:
  Authorization: Bearer <API_KEY>
```
## Response Format  
```
{
  "id": "12345",
  "title": "Example Movie",
  "release_date": "2025-01-23",
  "genres": ["Action", "Adventure"],
  "rating": 8.5,
  "cast": [
    { "name": "Actor Name", "role": "Lead Character" }
  ]
}
```

## Authentication  
```
Authorization: Bearer <API_KEY> 
```
Error Handling

The API returns standard HTTP status codes to indicate success or failure. Common error responses include:

400 Bad Request: The request was malformed or invalid.

401 Unauthorized: Missing or invalid API key.

404 Not Found: The requested resource could not be found.

429 Too Many Requests: Rate limit exceeded.

To handle errors effectively in your code:

```
Error Handling

The API returns standard HTTP status codes to indicate success or failure. Common error responses include:

400 Bad Request: The request was malformed or invalid.

401 Unauthorized: Missing or invalid API key.

404 Not Found: The requested resource could not be found.

429 Too Many Requests: Rate limit exceeded.

To handle errors effectively in your code:
```