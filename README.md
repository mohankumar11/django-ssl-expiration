# Django - Check SSL Expiration
# Introduction
> It's a Django application which completely checks 
>SSL expiration of host. Like if host has less than 15 days of 
>SSL expiration then, a message will be sent from sender email to all receiver email. Else, it will show "None of the host has less 
>than 15 days of SSL expiration".
## Getting Started

### Prerequisites
To send email, user should enable less secure apps and IMAP.
- [Python 3.5+]()
- [To send mail - Enable Less Secure Apps](https://myaccount.google.com/lesssecureapps)
- [Enable IMAP](https://mail.google.com/mail/u/0/?tab=rm&ogbl#settings/fwdandpop)

## Setup

The first thing to do is to clone the repository:

```sh
$ git clone https://github.com/Syed-Mujeeb/django-ssl-expiration.git

Create and activate a virtualenv:

virtualenv venv

source venv/bin/activate 

```

Then install the dependencies:

```sh
(venv)$ pip install -r requirements.txt

Once `pip` has finished downloading the dependencies:

```

Configure the SSL/settings.py
```sh
EMAIL_HOST_USER =  ' Sender_email_id '
EMAIL_HOST_PASSWORD =  '  Sender_password'
```

Configure the SSL/template/index.html
```sh
Change the value of sender email to the one which you given in settings. This will avoid confusion and help us to know from which email we are sending the emails
```

```sh
(venv)$ python manage.py runserver
```

And navigate to `http://127.0.0.1:8000/`.
