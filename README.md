# Hello Flask!

Simple Hello World using Flask

---

1. Install Flask
```bash
$ pip install flask
```

2. Install Apache2 and WSGI, Git
```bash
$ sudo apt-get install apache2 libapache2-mod-wsgi git
```

3. Clone this repo to `/var/www/` directory
```bash
$ git clone https://github.com/repodevs/hello-flask.git /var/www/hello-flask
```

4. Copy this `apache2/hello.conf` config to `site-available` apache2 directory
```bash
$ sudo cp apache2/hello.conf /etc/apache2/sites-available/
```

5. Enable configuration and disable default apache2 configuration
```bash
$ sudo a2dissite 000-default.conf
$ sudo a2ensite hello.conf
$ sudo service apache2 reload
```

6. Open in your browser [http://127.0.0.1](http://127.0.0.1)

