# django_cve_2019_19844_poc

PoC for [CVE-2019-19844](https://www.djangoproject.com/weblog/2019/dec/18/security-releases/)

![](https://github.com/ryu22e/django_cve_2019_19844_poc/workflows/django_cve_2019_19844_poc/badge.svg)

## Setup

1. docker-compose run --service-ports web python manage.py migrate --no-input
2. docker-compose run --service-ports web python manage.py createsuperuser --email=me@0xsha.io --username 0xsha
3. Head on to localhost:8000/accounts/password-reset
4. me@0xsha.ıo and hit enter (Note that "i" is malformed)
5. Check the console
