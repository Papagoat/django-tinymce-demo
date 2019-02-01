# Django Admin TinyMCE WYSIWYG Editor Demo

## Prerequisite
* Python => v3.7.2
* Virtualenv => v16.2.0
* Django => v2.1.5
* Django-tinymce => v2.8.0

## Installation

1. Download [Python](https://www.python.org/downloads/).


2. Install virtualenv

```sh
$ pip install virtualenv
```

3. Activate your virtualenv

**Windows**
```sh
$ virtualenv ENV
$ .\ENV\Scripts\activate
```

**Mac**
```sh
$ virtualenv ENV
$ source ./env/bin/activate
 ```

4. Install django and django-tinymce

```sh
$ pip install django django-tinymce
 ```
 or
 ```sh
 $ pip install -r requirements.txt
  ```

## Usage

cd into the demo directory and start the django server.
```sh
$ cd demo && python manage.py runserver
```
You may see an error in your terminal.

<span style="color:red">You have 15 unapplied migration(s). Your project may not work properly until you apply the migrations for app(s): admin, auth, contenttypes, sessions.
Run 'python manage.py migrate' to apply them.</span>

```sh
$ python manage.py migrate
```

Visit http://127.0.0.1:8000/admin from your browser.

We need to create an admin username and password before we can access the admin dashboard.

```sh
$ python manage.py createsuperuser
```

Click into *Demos -> Add Demo* and you will see that the TinyMCE WYSIWYG editor is loaded.

## Further reading
[django-tinymce documentation]https://django-tinymce.readthedocs.io/en/latest/
[Integration with django-filebrowser]https://django-filebrowser.readthedocs.io/en/latest/

## License
**MIT License**

Copyright (c) [2019] [Terence Lucas Yap]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
