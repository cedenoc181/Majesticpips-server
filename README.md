MajesticPips Backend Server

This is the backend server for the MajesticPips Discord community landing page. The server is designed to scrape real-time currency conversion data from the web, specifically converting $1 USD to other currencies, and providing this data to the frontend application. This backend supports the frontend by enabling users to see up-to-date conversion rates and facilitating community engagement through the Discord platform.


Technologies Used

Express.js: A fast and minimalist web framework for Node.js, used to handle routing and HTTP requests.

Puppeteer: A Node library that provides a high-level API to control Chrome or Chromium over the DevTools Protocol, used here for web scraping.

CORS (Cross-Origin Resource Sharing): Middleware used to enable cross-origin requests, allowing the frontend and backend to communicate even if they are hosted on different domains.