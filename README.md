# nest-local-dock

## Quick Overview
1. Clone nest-local-dock
    ```bash
    git clone https://github.com/dhtmdgkr123/nest-local-dock.git
    ```
2. Enter the nest-local-dock folder and rename .env.example to .env
    ```bash
    cp infra/dev/.env.example infra/dev/.env
    ```
3. Setting Your Project and env file
    1. setting your project path to
        ```code
        APP_CODE_PATH_HOST=../your/project/path
        ```

4. enjoy :)
    ```bash
    cd infra/dev
    docker-compose up
    ```

## Supported Services
1. NodeJs
2. Database Management Systems
    1. Mairiadb
3. Cache Engines
    1. redis
