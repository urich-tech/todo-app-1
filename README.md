# README
This is todo app used for creating task. It can be hosted on heroku using a postgresql database. It implements a CRUD structure( that is creat, read, update and delete) for data and has soft deletes(using discard gem). It is set to use Javascript web tokens(JWT) using the devise-jwt gem(segment of commented code for testing JWT if using API is included). It has been tested with postman and commented code is included for registering, logging in and signing out if testing the API.




Front page
![Screenshot_2023-01-01 TODOapp com Create TODO items activities](https://user-images.githubusercontent.com/69471917/210251856-e31f69ef-b473-4d64-b54d-d2f377d6681a.png)


Register
![Screenshot_2023-01-01 TODOapp com Create TODO items activities(1)](https://user-images.githubusercontent.com/69471917/210251864-3c9f6ff4-b036-4d38-a7ea-c0e20b7b8019.png)


Login
![Screenshot_2023-01-01 TODOapp com Create TODO items activities(2)](https://user-images.githubusercontent.com/69471917/210251871-83c56986-be6e-4105-aef0-765f2397c78f.png)


Dashboard
![Screenshot_2023-01-01 TODOapp com Create TODO items activities(3)](https://user-images.githubusercontent.com/69471917/210251875-29a08429-3bc1-4807-8e6c-051adce5817f.png)


Add task item board
![Screenshot_2023-01-01 TODOapp com Create TODO items activities(4)](https://user-images.githubusercontent.com/69471917/210251880-327ba5d6-8339-4e97-a053-64b6b1fc62fb.png)


User settings
![Screenshot_2023-01-01 TODOapp com Create TODO items activities(6)](https://user-images.githubusercontent.com/69471917/210251886-55d691e2-8f1b-462a-8d3f-e5e8c4ca7d04.png)


Annoymous users page
![Screenshot_2023-01-01 TODOapp com Create TODO items activities(7)](https://user-images.githubusercontent.com/69471917/210251892-0812b54c-d9ac-44ff-b395-66f9b9459923.png)

Things you may want to cover:

* Ruby version

Ruby 3.0.3


* System dependencies

rails 7.0.4


* Configuration

>bundle install


* Database creation
>rake db:migrate

* Database initialization

* Troubleshooting

If having error: abort rails! key not found:secret_key_base
clear or delete master.key and credentials.yml
run if using linux machine
>EDITOR="nano --wait" rails credentials:edit


* How to run the test suite
>bundle add rspec

>rails g rspec:install

>rspec


type in command prompt: rspec 
* Services (job queues, cache servers, search engines, etc.)


* Deployment instructions
>heroku login

>heroku create

>heroku rename todo-app

>git push heroku main

>heroku run rails db:migrate


# todo-app-jwt-authentication

User Login details


username: jondoe2@gmail.com

password: jondoe2


username: jondoe@gmail.com

password: jondoe




Docker settings:

To creat docker image
>docker build --tag mytodo .

>docker run -p 3000:3000 mytodo

>docker-compose up
