# Open Source Challenge Docker Setup

Clone this repo:
```bash
git clone https://github.com/opensource-challenge/development.git
cd development
```

Clone the API and the client inside this repo:
```bash
git clone https://github.com/opensource-challenge/opensource-challenge-api.git api
git clone https://github.com/opensource-challenge/opensource-challenge-client.git client
```

Start the project:
```bash
docker-compose up
```

#### Caveats (TODO fix these)
* In the client, to fix an error concerning `fetch` not being found, install `"whatwg-fetch": "3.3.1"` as an additional dependency.
* In the client, add the backend location in config/environment.js under ENV.APP.host = 'http://localhost:4000'
* In the API, in config/dev.exs, add `hostname: "db"` to the database configuration
