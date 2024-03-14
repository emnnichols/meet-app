# Meet app

## Description
The Meet app is a serverless, progressive web application that uses React and a
test-driven development technique. The application uses the Google
Calendar API to fetch upcoming events.

## Key Features

### Filter Events by City

#### - As a user, I should be able to filter the events so that only events happening in that city are shown

#### - Given the user hasn’t searched for a specific city
  - When a user opens the app
  - Then the app should list events happening in all cities

#### - Given the main page is open
- When a user starts typing a city
- Then the user should receive a list of suggestions that match what they’ve typed

#### - Given a user typed a city in the search box and their are suggestions being shown
- When a user clicks on a city from the suggestions
- Then the users city should change and the app should show events from that city


### Show/Hide Event Details

#### As a user, I should be able to show/hide details of events so that I can control how much information is shown to me.

#### - Given the app is opened
- When a user looks through the list of events
- Then the event details should be collapsed

#### - Given a user wants to see details about a specific event
- When a user clicks on the details button
- Then the event element is expanded to show details

#### - Given a user wants to hide the event details
- When a user clicks on the hide button
- Then the event element is collapsed to hide the details


### Specify Number of Events

#### - As a user, I should be able to choose the number of events shown to me so that I can easily look through the events 

#### - Given a user doesn’t specify a number of events to show
- When a user loads the app to look at events
- Then only 32 events will be shown

#### - Given a user wants to change the number of events shown
- When a user changes the number from the default 32
- Then the list will update to show the number of events the user chose


### Use the App When Offline

#### - As a user, I should be able to have offline access to the app so that I can still find information on events even when I don’t have an internet connection.

#### - Given there is no internet connection
- When the user opens the app
- Then they will be shown a cached version of the data

#### - Given these is no internet connection
- When the user tries to change search settings (like the city or number of events shown)
- Then the app will show an error


### Add an App Shortcut to the Home Screen

#### - As a user, I should be able to create a shortcut to my home screen so that I can have quick access to the app.

#### - Given the app is open
- When a user chooses to add the app the their home screen
- Then a shortcut to the app will be added to their home screen


### Display Charts Visualizing Event Details

#### - As a user, I should be able to view charts that visualize event details so that I can easily compare data about events in a clear and concise manner.

#### - Given the user wants to see or compare upcoming events in each city
- When the user navigates to the chart section of the app
- Then they can see the number of upcoming events in each city
