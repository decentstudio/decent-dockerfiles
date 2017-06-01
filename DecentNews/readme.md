Launch the DecentNews application environment.

1. Follow `docker build` instructions for the decent-slack-receiver.
2. Follow `docker build` instructions for the decent-news-distributor.
3. Set up `.env` file based on the `.env.example` file in this directory.
3. `docker-compose up -d`
4. Hit `localhost:8081/api/news` for an empty JSON response.
