LAB 14: Event Driven Applications
Codefellows 401 JavaScript

Project: Socket-io Team App

Overview
Spent 2 days collaborating to create a chatroom and speed typing minigame. From a central server socket, multiple clients are able to join over a hosted network. Upon connection, each client is able to assign themselves a username which is displayed upon any message input into the terminal. This message is sent to the server, then bounced back to all clients currently connected, creating a realtime messaging service. 

Features:
an event listener tracks certain commands able to be entered by the user:

data(dev command) - displays to the server information about the current server, who is playing, all clients' usernames, and current scores of all players.
start - any user may enter start to begin the speed typing mini game. after a short countdown, a tongue twister is sent to all players connected to the current space.wWhomever types the response that matches the displayed message the fastest wins a point for that round. After one player has earned three points, they are declared the winner.
terminal is cleared of entered text and output from previous game rounds to keep a clean looking display for better user experience.

Authors
Mike Greene
Jenner Dulce
Ryan Tipper

Links and Resources

dependencies:
socket.io
socket.io-client
repl
Setup
Assign the server.js a host server route
Assign a 'username' in client.js and ensure the host being connected to matches the route provided to server.js
.env requirements (where applicable)
N/A
How to initialize/run your application
node server.js to create the server.
node client.js to connect to the host server.
type your messages in the terminal and hit enter to chat in real time
type 'start' to begin the minigame, a countdown will begin and then send a message to all clients.
type the exact message and send it back in order to win, whomever can type the message the fastest wins the round.
after one player wins three rounds, the game declares them the victor.
debug messages are displayed in the server.js console, type 'data' at any time to get information about all clients currently connected.
© 2021 GitHub, Inc.
