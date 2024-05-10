## How to install
1. Clone the following github with the command
```
git clone https://github.com/kamalfikrikamal/Laravel-Reactjs-Docker
```
2. Open Docker Desktop and make sure it is running.
3. Run the following command on the terminal in the github folder that has been cloned.
```
docker-compose up -d --build
```

4. When finished, duplicate the .env.example file into .env and change the .env file in the required section.
```
cp .env.example .env
```
5. If so, open Docker Desktop. In the Containers menu, select the laravelreactjs container that was created, then select laravelreactjs-app. Open the Terminal tab and run the following commands in sequence.
```
composer install
```
```
php artisan key:generate
```
```
php artisan migrate
```
```
php artisan db:seed
```
```
npm run dev
```
6. To access the application, you can directly open the browser with IP
```
http://localhost
```
7. To access phpmyadmin, you can directly open a browser with IP
```
http://localhost:8081
```