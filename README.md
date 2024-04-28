# Bakend Developer Capstone Project

## Project Overview

This project serves as the final assignment for the Backend Developer Capstone Course within the Meta Backend Developer Professional Certificate on Coursera. The project consists of two main apps: `api` and `restaurant`. The `api` app provides API endpoints, while the `restaurant` app serves as the frontend. The project structure includes a `config` directory holding major settings.

## Installation

To install the project dependencies, run:

```
pipenv install
```

## Setup
Adjust the database settings in the config/settings.py file according to your local setup. Then apply migrations.

## Environment Variables

For authenticated API requests in the view of the restaurant app, provide a username and password in a .env file within the restaurant app folder:

```
USERNAME=your_username
PASSWORD=your_password
```

Ensure django-environ is installed.

## API Endpoints

API Endpoints
The api app has a total of 4 endpoints. Additionally, Djoser and SimpleJWT endpoints are available.

Each endpoint requires a SimpleJWT Token for authorization. Pass the token in the header of the request such as



```{'Authorization': 'JWT <token>'}```

In Insomnia, add the token as follows
<br />
![image](https://github.com/theskysinha/Meta-Backend-Capstone-Project/assets/66449020/0a9c86c2-b5bd-4d55-827f-96129354b90f)

```
http:127.0.0.1:8000/api/menu-items
http:127.0.0.1:8000/api/menu-items/{menu-itemId}
http:127.0.0.1:8000/api/bookings
http:127.0.0.1:8000/api/bookings/{bookingId}
```

Endpoints for djoser app

http://127.0.0.1:8000/auth/users/
http://127.0.0.1:8000/auth/users/me/
http://127.0.0.1:8000/auth/users/confirm/
http://127.0.0.1:8000/auth/users/resend_activation/
http://127.0.0.1:8000/auth/users/set_password/
http://127.0.0.1:8000/auth/users/reset_password/
http://127.0.0.1:8000/auth/users/reset_password_confirm/
http://127.0.0.1:8000/auth/users/set_username/
http://127.0.0.1:8000/auth/users/reset_username/
http://127.0.0.1:8000/auth/users/reset_username_confirm/
