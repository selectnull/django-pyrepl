django-pyrepl
=============

You've upgraded your Django project to Python 3.13 and want to try out the
new REPL. Unfortunately, it's a no go. But thankfully, Trey Hunner wrote
[Django and the Python 3.13 REPL](https://treyhunner.com/2024/10/django-and-the-new-python-3-dot-13-repl/)
article in which he shows how to enable it.

This is just his idea packaged into a installable django app.
Full credits go to Trey.

Warning: This app uses unsupported `_pyrepl` module. Hopefully,
the future versions of Python will be supported and this app
becomes deprecated.

## Installation

```bash
uv add django_pyrepl
```

Or if you really need to:

```bash
pip install django_pyrepl
```

After that, simply add it to `INSTALLED_APPS` in your project `settings.py`

```python
INSTALLED_APPS = [
    ...
    "django_pyrepl",
    ...
]
```

## Licence

MIT.
