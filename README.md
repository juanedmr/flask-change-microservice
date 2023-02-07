
# flask-change-microservice
Small Flask Microservice deployed with docker


## Invoke Endpoint

* Create virtualenv and source it: `python3 -m venv ~/.fcm && source ~/.venv/bin/fcm`
* Install and Test:  `make all`
* Run it:  `python app.py`
* Invoke it.  This is to check everything is ok. Starting the flask app


### Curl

`curl http://127.0.0.1:8080/change/1/34`

```bash
[
  {
    "5": "quarters"
  }, 
  {
    "1": "nickels"
  }, 
  {
    "4": "pennies"
  }
]
```

### Docker

* Run `make build` in order to create your docker image.
* Verify it runnig `docker image ls`
* Run the app in the container using `make run`

