
# Wikipedia Search Application

## Overview
This is a simple web-based Wikipedia search application that fetches and displays search results from Wikipedia using an API. The application allows users to enter a search term, fetch results dynamically, and display them in a structured format.

## Features
- Search for Wikipedia articles using keywords.
- Display search results with titles, links, and descriptions.
- Show a loading spinner while fetching results.
- Open search results in a new tab.

## Technologies Used
- HTML
- CSS
- JavaScript
- Fetch API

## How It Works
1. The user types a search term into the input field and presses the **Enter** key.
2. A request is sent to the Wikipedia API endpoint to fetch related search results.
3. While waiting for results, a spinner is displayed to indicate loading.
4. The fetched results are displayed dynamically with titles, links, and descriptions.
5. Clicking on a search result opens the Wikipedia page in a new tab.

## Code Explanation
- `searchInputE1`: Captures user input.
- `searchResultsE1`: Holds the dynamically generated search results.
- `spinnerE1`: Displays a loading spinner while data is being fetched.
- `searchWikipedia(event)`: Triggers the API request when the **Enter** key is pressed.
- `displayResults(searchResults)`: Handles displaying search results on the webpage.
- `createAndAppendSearchResult(result)`: Creates and appends each result to the search results section.
- Uses the `fetch` API to retrieve data from the Wikipedia search endpoint.

## API Endpoint
The application fetches data from:
```
https://apis.ccbp.in/wiki-search?search=<search-term>
```

## Setup and Usage
1. Clone the repository or copy the code.
2. Open the HTML file in a web browser.
3. Type a search term and press **Enter** to fetch results.

## Example Search
If the user searches for "JavaScript," the API returns:
```json
{
  "search_results": [
    {
      "title": "JavaScript",
      "link": "https://en.wikipedia.org/wiki/JavaScript",
      "description": "JavaScript is a programming language used for web development."
    }
  ]
}
```
The webpage will display the result with a clickable title, URL, and description.

## License
This project is open-source and free to use.


