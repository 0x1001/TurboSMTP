# TurboSMTP client

TurboSMTP (http://serversmtp.com) is online service for sending emails. TurboSMTP client is very simple Python library for using online API of this service. The difference between this client and client provided by serversmtp.com (http://www.serversmtp.com/en/smtp-api) is in a way how e-mail messages are handled. This library supports python built-in email module, which makes composing complex e-mail messages much easier.

To use this module you have to have account at http://serversmtp.com . Basic account is free of charge.

## Version
1.0.1

## Installation
```sh
$ pip install turbosmtp
```

## Usage
```python
import turbosmtp
from email import message

message = message.Message()
message["From"] = "from@address.com"
message["To"] = "to@addresss.com"
message["Subject"] = "Hello World!"

smtp = turbosmtp.TurboSMTP("your_username", "your_password")
smtp.send(message)
```

## Want to contribute?

Anyone is welcome to contribute to this project :). 
Just contact me on Github.

## License
GNU GENERAL PUBLIC LICENSE

