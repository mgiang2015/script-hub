# Python Config Manager Script

Web applications usually need different  configurations for development, staging, and production environments such as database URLs, API keys, and debug. This script reads from `config` folder and generates environment-specific config files which can then be read by application.

## Support

- Reads `.yaml` files as input configuration
- Output `.env`, `config.json` and `docker-compose.env` files for each environment provided

## Features

- Supports `${VAR_NAME}` syntax for secrets in staging/prod
- Works with different data types such as booleans, arrays
- Flattens nested configurations