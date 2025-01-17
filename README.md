# api-tester: a Test Website for testing Discogs API
First test of Discogs API

### User Token vs OAuth

Using the User Token authentication method since we do not (at this point) need to access User-specific data, just data that is generally available to the public.

### Python Library

Using the discogs_client library [https://github.com/joalla/discogs_client](https://github.com/joalla/discogs_client)

## To run on local machine

### get a User-Token from Discogs

“Click user avatar on top right of screen” - “Settings” - “Developers” - “Generate new token “. Directions from [https://python3-discogs-client.readthedocs.io/en/latest/authentication.html#user-token-authentication](https://python3-discogs-client.readthedocs.io/en/latest/authentication.html#user-token-authentication).

### set up a local venv

Run `python3 -m venv env` or similar command to instantiate a new virtual environment.

Then run `source env/bin/activate` to enter that environment

Finally run `pip3 -r requirements.txt` or similar to get all libraries in the requirements.txt file

### export the token variable

Then take the User-Token from Discogs and run `export USER_TOKEN="whatever-the-token-is"` with the token inside the quotation marks.

### run Flask

Finally run Flask by going into the directory of the repo and running `flask run`