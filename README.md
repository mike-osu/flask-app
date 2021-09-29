# flask-app

This app is running at [http://flip3.engr.oregonstate.edu:1599](http://flip3.engr.oregonstate.edu:1599)

## Start/stop app:
SSH into flip server, run commands at project's root folder

Start Flask app on OSU server
```
gunicorn --bind 0.0.0.0:1599 wsgi:app -D
```

List processess
```
ps ax | grep gunicorn
```

Stop Flask app
```
kill [number running app's gunicorn process]
```
