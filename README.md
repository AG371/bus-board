# bus-board
An online booking system for bus tickets in Kenya

# Bus Board

## By **[Gitu Mbugua(https://github.com/GituMbugua)]**, **[John Mutavi(https://github.com/jonnygovish)]** and **[Carol Wanjohi](https://github.com/carolwanjohi)**

## Description
[This]() is a web application that allows users to search for buses by entering their starting point and destination. The results list has buses arranged with the cheapest bus at the top of the list. The user can select a bus and book a seat in the bus.

## User Stories
As a user I would like to:
* see some of  the available routes
* search for a bus by entering the departure location and arrival location
* select a route
* see buses on the selected routes, number of buses, ticket price and timings
* select a bus
* create an account
* be directed to the login page after clicking select
* see information on the selected bus
* see the Paybill number after clicking book

## Specifications
| Behavior        | Input           | Outcome  |
| ------------- |:-------------:| -----:|
|  |  |  |

## Setup/Installation Requirements

### Prerequisites
* Python 3.6.2
* Virtual environment
* Postgres Database
* Internet


### Installation Process
1. Copy repolink
2. Run `git clone REPO-URL` in your terminal
3. Write `cd bus-board`
4. Create a virtual environment with `virtualenv virtual` or try `python3.6 -m venv virtual`
5. Create .env file `touch .env` and add the following:
```
SECRET_KEY=<your secret key>
DEBUG=True
```
6. Enter your virtual environment `source virtual/bin/activate`
7. Run `pip install -r requirements.txt` or `pip3 install -r requirements.txt`
8. Create Postgres Database

```
psql
CREATE DATABASE bus-board
```
9. Change the database informatioin in `/settings.py` 
```
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'bus-board',
        'USER': *POSTGRES_USERNAME*,
        'PASSWORD': *POSTGRES_USERNAME*,
    }
}
``` 
10. Run `./manage.py runserver` or `python3.6 manage.py runserver` to run the application

## Known Bugs

* search for buses by routes
* select a bus
* book a bus

## Technologies Used
- Python 3.6.2
- Django 1.11.7
- Google Maps API
- Bootstrap 3
- Postgres Database
- CSS
- HTML
- Heroku

### License

MIT (c) 2017 **[Gitu Mbugua(https://github.com/GituMbugua)]**, **[John Mutavi(https://github.com/jonnygovish)]** and **[Carol Wanjohi](https://github.com/carolwanjohi)**




