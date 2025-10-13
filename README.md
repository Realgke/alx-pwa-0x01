# ALX Project 0x14 - MoviesDatabase API Documentation Review

## API Overview
The **MoviesDatabase API** provides access to an extensive collection of movie data, including details about films, TV shows, actors, genres, ratings, and production information. It allows developers to search for movies, retrieve metadata such as release dates, plot summaries, and cast lists, and explore related resources like similar movies or trending titles.

Key features include:
- Search functionality for movies, TV shows, and people.
- Access to detailed information such as runtime, genres, cast, and crew.
- Support for pagination and filtering in API responses.
- Provides structured JSON data for easy integration into applications.

---

## Version
**API Version:** 1.0.0

---

## Available Endpoints

| Endpoint | Description |
|-----------|--------------|
| `/titles` | Fetches movie and TV show titles. Supports searching and filtering. |
| `/titles/{id}` | Retrieves detailed information about a specific title by its unique ID. |
| `/titles/search/title/{query}` | Searches for a movie or show by title name. |
| `/titles/series/{id}` | Retrieves series information, including all episodes under a show. |
| `/actors/{id}` | Fetches information about a specific actor or actress. |
| `/genres` | Lists available movie and TV show genres. |
| `/titles/random` | Returns a random movie or show entry. |

---

## Request and Response Format

### Example Request
```bash
GET https://moviesdatabase.p.rapidapi.com/titles
Headers:
  X-RapidAPI-Key: your_api_key_here
  X-RapidAPI-Host: moviesdatabase.p.rapidapi.com
