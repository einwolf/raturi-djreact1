# Django with webpack and react

Django rendering react through webpack. Django uses django-webpack-loader. Node uses webpack-bundle-tracker.

https://raturi.in/blog/multi-page-web-application-using-django-react-and-webpack/

https://github.com/raturitechmedia/django-react-webpack

## Django commands

```bash
# Django setup
django-admin startproject djpack

# Django dev
python manage.py migrate
python manage.py runserver 0.0.0.0:8000
```

## Nodejs commands

```bash
# Nodejs setup
# Install npm into frontend directory
cd djaccord/frontend
npm install
npm install react react-dom

# Run nodejs in watch mode
npm run watch
```

## Django urls

http://127.0.0.1:8000/

## Nodejs urls

http://127.0.0.1:8080/
