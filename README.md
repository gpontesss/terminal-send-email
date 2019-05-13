# Send Email utility
This is a simple script for sending emails to an address list through the terminal. It requires a JSON file `to-address.json`, that contains the mailing list. It sends data redirected to its stdin.
It also requires a `email.env` file with configuration variables.

## Using it
You may want to run `pip install -r 'requirements.txt'`.
```bash
    echo "This is coming from the terminal!" | ./send-email
```