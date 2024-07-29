# mf-tutorial-amar

Commands:
ng new mono-workspace --create-application=false
ng g application host-app --routing --style=scss --ssr=false --standalone=false
ng g application mfe-app --routing --style=scss --ssr=false --standalone=false

ng s host-app -o
ng s mfe-app -o

npm i webpack webpack-cli --save-dev
ng add @angular-architects/module-federation --project host-app --port 4200
ng add @angular-architects/module-federation --project mfe-app --port 4300

ng g c home --project=host-app
ng g c todo --project=host-app


