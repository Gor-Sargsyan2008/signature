# WorkShop backend
Backend application for Workshop.

A REST service on python Flask framework.

# Local development

## Requirements

- [Python 3.8](https://www.python.org/downloads/) or higher
- [Docker](https://docs.docker.com/engine/install/) and [Docker Compose](https://docs.docker.com/compose/install/)

## Run on local machine
Create a virtualenv

```shell script
virtualenv venv
```

Activate virtualenv

```shell script
source venv/bin/activate
```
Start docker-compose services

```shell script
sudo docker-compose up -d
```

For Database initialization

```
flask db init
```

Install  dependencies


```shell script
pip install -r requirements.txt
```

Copy the `.env.example` file to `.env` and change configuration to appropriate values

```shell script
cp .env.example .env
```

Run the migrations

```shell script
flask db upgrade
```

Start the application locally

```shell script
flask run
```

## Running tests

```shell
python -m unittest discover tests
```

```shell
python -m coverage run -m unittest discover
```

```shell
python -m coverage html
```

For creating a new migration

```shell script
flask db migrate -m "migration message"
```


## Environment variables
| Variable                       | Description                                                   |
| -------------                  |:-------------:                                                |
| Some var                       | description .                                                 |

6fa126be-474d-4438-b8c2-d181e4c9456c

secret-key
fee0d13c-02f3-44fb-b87a-77d90916fa24

Integration Key
c4582fd4-19e1-4c78-88e2-3584ba033727

URL structure
https://account-d.docusign.com/oauth/auth?response_type=code&scope=signature&client_id=c4582fd4-19e1-4c78-88e2-3584ba033727&redirect_uri=http://127.0.0.1:5000/documents/code
