# Django with webpack and react

Django rendering react through webpack. Django uses django-webpack-loader. Node uses webpack-bundle-tracker.

https://raturi.in/blog/multi-page-web-application-using-django-react-and-webpack/

https://github.com/raturitechmedia/django-react-webpack

## Django commands

```bash
# Django setup
django-admin startproject djwebpack
mkdir djwebpack/templates

# Django dev
python manage.py migrate
python manage.py runserver 0.0.0.0:8000
```

## Nodejs commands

```bash
# Nodejs setup
mkdir djwebpack/frontend
cd djwebpack/frontend

npm install --save-dev @babel/cli @babel/core @babel/preset-env @babel/preset-react @babel/register babel-loader
npm install --save-dev webpack-cli webpack webpack-bundle-tracker
npm install react react-dom react-scripts
npm install @testing-library/jest-dom @testing-library/react @testing-library/user-event

# Run nodejs in watch mode
npm run watch
```

## Django urls

http://127.0.0.1:8000/

## Nodejs urls

http://127.0.0.1:8080/
