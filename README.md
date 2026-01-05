# Microforntend-Apps
Microfrontend

0. Generate 3 projects:

ng new movie-ticket
ng new movie-list
ng new ticket-availability

1. install native federation for all 3 projects must be mention @19 else there will be verion issue:

npm install @angular-architects/native-federation@19

2. generate & initialise the native federation for all 3 apps:

ng g @angular-architects/native-federation:init --project movie-ticket --port 4200 --type dynamic-host

ng g @angular-architects/native-federation:init --project movie-list --port 4201 --type remote
ng g @angular-architects/native-federation:init --project ticket-availability --port 4202 --type remote

5. create service for main app(movile-ticket)
ng g s micro-frontend

6. run applications: 
movie-ticket:

ng serve 

movie-list:
ng server --port 4201

ticket-availability:
ng server --port 4202

