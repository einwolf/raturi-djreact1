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

# Run nodejs in watch mode to rebuild files
cd djwebpack/frontend
npm run watch

# Static build all bundles once
cd djwebpack/frontend
npm run build
```

## Django urls

<http://127.0.0.1:8000/>

Regular

<http://localhost:8000/default/>
<http://webstatusproj:8000/static/static_test.html>

React

<http://localhost:8000/index1>
<http://localhost:8000/index2>

## Nodejs urls

It's supposed to server webpack bundles through django. Not like through webpack-build-server.

The frontend/src and frontend/public probably came from create-react-app.
The files aren't directly used by index1.html.

<http://127.0.0.1:8080/>
