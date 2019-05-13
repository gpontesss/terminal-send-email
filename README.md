# Send Email utility
This is a simple script for sending emails to an address list through the terminal. It requires a mailing list with target email addresses. It can send messages passed through `stdin` or specifying a filename with proper content.
It also requires a `email.env` file with configuration variables. See `email.env.default` and configure values accordingly.

## Usage
You may want to run `pip install python-dotenv` before using it. You can find basic usage instructions with `./send-email --help`:
```bash
usage: send-email [-h] [-b body_message] [-t email_title] -ml
                  addresses_filename

Send emails via cli.

optional arguments:
  -h, --help            show this help message and exit
  -b body_message, --body body_message
                        Name of file containing body message. It can also be
                        passed through pipes to stdin.
  -t email_title, --title email_title
                        Title of the email.
  -ml addresses_filename, --mailing-list addresses_filename
                        Name of file containing mailing list. Can be a JSON
                        list file.
```