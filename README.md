# WP Bedrock

WordPress docker project built on top of [Bedrock](https://roots.io/bedrock/) with WP Media Cloud integration.

## Features:
- Environment variables.
- Separate configs per environment.
- Composer for managing WordPress installation.
- Composer for managing WordPress plugins and themes.
- WP Cli Integration.
- Persistent data storage.
- WP Media Cloud integration.

## Installation

 1. Clone the repository to your local machine: ``` git clone   
    https://github.com/amurinn/wpbedrock.git ``` 
 2. Navigate to /root folder and run ``` composer install ```
 3. Add `127.0.0.1 wpbedrock.docker` to your hosts file.
 4. Rename `.env.example` to `.env`, most values are already filled, but you will need to provide google cloud bucket name in case you want to use WP Media Cloud right away.
 5. Rename `bucket-credentials.example.json` to `bucket-credentials.json`, and replace values with bucket credentials.
 6. Run `docker compose -f docker-compose-dev.yml up --build`
 7. Open http://wpbedrock.docker/ in the browser and install WordPress.
 8. Enjoy ;)
