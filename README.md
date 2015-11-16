# Youtube Live Dashboard

## Use Case

Client A would like to view all relevent live streaming analytics in real-time, on a custom dashboard. 

## Task

Create a real-time, live analytics dashboard using a Youtube Live stream channel as the source. The data on this page should update as frequently as possible and should provide user A with the ability to understand the performance of their live event.

## Tools

* Youtube API
	* Specifically the Analytics and Data API
* Ruby on Rails
* ~~We'll be using [*NASA Video : Earth From Space Real Footage - Video From The International Space Station ISS*](https://www.youtube.com/watch?v=njCDZWTI-xg) as our source.~~
	* We can only see data from our own streams.
		* This will make testing difficult...

## Deliverables

* Code for the project
* Link to the project

## Steps
1. Research Youtube API
	1. Figure out what analytics data is available
		1. Follow a Tutorial to see how to properly utilize the API
	2. Decide which ones are useful
2. MVP
	1. Display all useful analytic data staticly
	2. Figure out how to update the data without the page reloading
		1. Find out which metrics are most expensive to call repeatedly so that we don't go over the quota and get locked out
3. Styling
	1. Add in Bootstrap
	2. ???

# Notes and Musings

* We'll be using the YouTube Analytics API so that we can get real time data instead of the YouTube Reporting API which would give us lots of data in bulk.
* We won't need a database since our dashboard is just supposed to populate with data in real time.
	* Javascript static page?
* We might need authorization in order to see a channel's specific data.
	* Alternatively we could be the channel's owner therefore bypassing the need for authorization.
* The tutorial has the whole authorization process which will be necessary for the dashboard as well.
* The tutorial also uses Google Visualization, so should be able to use that to show the data on the dashboard in a meaningful way.
* Testing the API to make sure it is correctly returning data is turning out to be quite tough since I don't have a YouTube presence with the developer account.
	* Need to find some way to authorize developer account on other barely started YouTube account.
