# API DOCS

## Running the server locally

1. First, clone the repo
2. After cloning the repo, run `npm install`
3. In the terminal at the base director of the project, run `npm start`. This will start the node server with nodemon. The server will be running on local host 3001. You should see a message is running in the dev console to confirm the server is up and running.

## Api Routes (local)

localhost:3001/api/heartbeat [GET]
returns 200 status code and the following JSON `{ "message": "api up and running"}`

localhost:3001/api/groceryitems [GET]
returns 200 status code and all the grocery items from the data base along with the number of results

can add queries to url to filter results
q=[string that searches through the names of grocery items]
store=[must be walmart or marketstreet] -> will add more later
minor_category=[must be chicken or groundBeef] -> will add more later

example request
localhost:3001/api/groceryitems?q=family&store=walmart&minor_category=groundBeef
