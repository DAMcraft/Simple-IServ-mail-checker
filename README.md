# Simple-IServ-mail-checker
Simple checker using the IServ mail-API to see if an email exists. Useful for scraping. 

## Usage
```python
from iserv import iserv

iServ = iserv('iserv-instance.de')
iServ.login(username, password)

# Check if email exists
iServ.check_email(name)

# Get autocomplete suggestions
iServ.get_autocomplete(name)
```

## Methods
- `login(username: str, password: str) -> 'iserv'`: Login to iServ using the given credentials.
- `check_email(name: str) -> bool`: Check if an email address exists for the given name.
- `get_autocomplete(name: str) -> list`: Get a list of autocomplete suggestions for the given name.
