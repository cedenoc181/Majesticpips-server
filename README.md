~MajesticPips Backend Server

This is the backend server for the MajesticPips Discord community landing page. The server is designed to scrape real-time currency conversion data from the web, specifically converting $1 USD to other currencies, and providing this data to the frontend application. This backend supports the frontend by enabling users to see up-to-date conversion rates and facilitating community engagement through the Discord platform.


~Technologies Used

Express.js: A fast and minimalist web framework for Node.js, used to handle routing and HTTP requests.

Puppeteer: A Node library that provides a high-level API to control Chrome or Chromium over the DevTools Protocol, used here for web scraping.

CORS (Cross-Origin Resource Sharing): Middleware used to enable cross-origin requests, allowing the frontend and backend to communicate even if they are hosted on different domains.


~Features

Real-Time Currency Conversion Scraping: The server scrapes currency conversion rates from the website FT Markets to provide the current value of $1 USD in other currencies.

Caching: The server caches the scraped data for 1 minute to reduce the number of requests made to the source website and improve response times for the frontend.

Error Handling: The server includes basic error handling to manage any issues that arise during the scraping process.

~API Endpoints

-GET /scrape

Scrapes real-time currency conversion data and returns it as a JSON response. The data is cached for 1 minute to optimize performance.

-example response from server fetch

[
  {
    "name": "USD/EUR",
    "abbreviation": "USD",
    "conversions": "0.85"
  },
  ...
]


Installation & Setup

To run this server locally:

Clone the repository:

-copy this code into the CLI (SSH):

git clone git@github.com:cedenoc181/Majesticpips-server.git

Navigate to the project directory:

-change directory to <project-directory> in CLI with input below:

cd project-directory

Install the dependencies:

-enter to CLI:

npm install

Start the server:

-enter to CLI:

Node server.js

The server will be running on http://localhost:3001/scrape.
