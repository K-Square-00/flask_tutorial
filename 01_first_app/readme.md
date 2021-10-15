# Setup first Flask app

1. install Flask

```
mkdir myproject
cd myproject
python3 -m venv venv
```

2. create hello world script (e.g. hello.py)
```
from flask import Flask

app = Flask(__name__)

@app.route("/")
def hello_world():
    return "<p>Hello, World!</p>"

```

3. Set FLASK_APP varialbe with filename of the script (e.g. hello). **Note:** Ensure the current directory is where the script is located.  
```
export FLASK_APP=hello
flask run
```

4. Now head over default URL and you should see your hello world greeting.
```
http://127.0.0.1:5000/
```


