## Objective
The main objective of creating this project was to understand the concept of broadcasting. I have taken help of this tutorial https://www.youtube.com/watch?v=CkRGJC0ytdU by Scrypster. 

## Learning  
Broadcasting is very important to build real time applications like this one. Through this project I understood how to setup events and listeners. Events are broadcasted on channels (here pusher channels are being used) and listening is handled by laravel echo (a js library integrated with pusher-js) to listen on channels for various events.

## Challenges
The pusher keys generated from your account on pusher.com are to be configured in your .env file. However the challenge I faced was reading these values into bootstrap.js . I used process.env.MIX_PUSHER_APP_KEY to read in environment variables . This doesn't work for some reason so I had to hard code these values. I am still trying to find a way around it.

## Technologies used
- Vue.js for front-end
- Laravel for back-end
- an account on pusher.com for building websocket connections
- Laravel echo with pusher-js to listen on the channels for events
