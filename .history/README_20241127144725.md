This a baseline dev enviroment for web dev with a redis and a database setup for access. It can be used across multiple projects as long as DB names are different and each redis entry is prepended with a unique value.

# Component overview
- MSSQL server
    - Port 1433 accessible via tcp (likely needs to be forced locally)
    - should be accessible through http://localhost:1433
    - User: SA
    - Password: Password12!
- Redis
    - Accessible through port 6379 and http://localhost:6379
- Redis Commander
    - Frontend to inspect redis content
    - accessible through http://localhost:9666

# Instructions
- Requires a WSL2 linux environment and docker
- Open this folder with your cmd and run `docker-compose up -d` 
    - Run `docker-compose up` if you want to see the logs, its preferable to not do this, and instead attach to the containers later
