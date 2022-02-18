# AuthGG

Python lib for dealing with Auth.gg api

## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install requests

Add the auth.py file in your application folder

## Usage

```python
from auth import *

# Adds the application information to the base
AuthGG.__init__(
    aid="AID",
    apikey="API_KEY",
    secret="SECRET_KEY"
)

# Returns the output of the request
response: str = AuthGG.Action(
    _type="login",
    username="Username", password="Password",
    hwid="hwid"
)
print(response, end='', flush=True)
```

### Auth.GG
```
Website: str = "https://auth.gg/"
