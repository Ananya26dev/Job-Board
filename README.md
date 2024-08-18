# Job Board

Build a job board that displays the latest job postings fetched from the Hacker News API, with each posting displaying the job title, poster, and date posted.

Requirements

The page should show 6 jobs on initial load with a button to load more postings.
Clicking on the "Load more" button will load the next page of 6 postings. The button does not appear if there aren't any more postings to load.
If there's a url field returned for the job details, make the job title a link that opens the job details page in a new window when clicked.
The timestamp can be formatted in any way you like.

API

Hacker News has a public API to fetch jobs by Y Combinator companies. There's no single API that fetches a list of jobs together with the data, so you will have to make separate requests to fetch the necessary data and combine them to be displayed.

Job Stories

Fetches a list of job posting IDs.

URL: https://hacker-news.firebaseio.com/v0/jobstories.json
HTTP Method: GET
Content Type: json

Job Details

Fetches job posting details given its ID.

URL: https://hacker-news.firebaseio.com/v0/item/{id}.json
HTTP Method: GET
Content Type: json
Sample response for https://hacker-news.firebaseio.com/v0/item/35908337.json:
