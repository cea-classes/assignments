# Module 2 Assignments

Module 2 itself will be one big project with lots of parts in it. It will be a multipurpose bot with lots of functionalities. Module 3 will also depend a lot on module 2.

## Indeed.com scraper

Create a web service with an api that searches indeed.com or monster.com for latest "Remote" jobs. 

Data to collect:
- Job title
- Job URL
- Unique ID
- Description
- Apply Button URL
- Date posted

Rules:
- It should avoid adding the jobs that's already in database.
- This should paginate upto 5 page using normal or "load more" pagination.

The scraper should have two operating modes. 
- Scheduled mode: it will scrape the website for new jobs all of the time (every 24 hours), and save data to db.
- On Demand mode: it will scrape the website for specific keyword when requested.

## API and database

Create an API that can be used later for multiple scraper services.

The API will have three modes:
- Database Mode: return the result from database. 
- Queue mode: queue the task and return the data using websocket and further api call.
- Realtime mode: returns the result from the website and save data to db at same time.

Optional:
- A frontend is optional but highly recommended. 
- Integrate algolia/elasticsearch or any text based search to the api.

## Create various scrapers

- Extract data from example.com
- Login to a website and using cookies
- Normal next pagination 
- Normal infinity pagination
- Fill SSO and 2FA
- Search in Amazon, Google, Booking, Youtube, Duckduckgo
- Checkout in shopify, walmart
- Scrape review from facebook, google, yelp

## Bypassing bot prevention and limitations

- Using a Proxy
- Using a VPN
- Faking the location and language
- Solving a captcha

## Extra - Zapier web automation

- Create a minimal slack bot
- Simple html form to google sheet workflow
- Google form to facebook workflow

# Module 3

This will be continuation of module 2 project.

## Host the scraper in docker

- Implement docker and compose code in the codebase
- Run scraper with virtual display
- (Optional) Run scraper in server

## Tests

- Create/update a basic UI
- Add minimal test for the UI

## CI/CD

- Deploy to server using github actions
- Run tests using github actions
