# Snapcast with Spotify, Airplay & Swedish Radio

My parents old computer broke which we used for playing music at home. I wanted to solve this. We have some "dumb" speakers and a raspberry pi without usage.
Then I saw Snapcast, which got me started working on this.
**This is a ongoing project! I started with documentation and research. I will add images and products bought when I have started assembling the project.**

## Hardware used

This is the hardware I used for this project. Snapcast is very flexible, so use what you have.

- Raspberry Pi 3B as client
- DAC for Raspberry Pi. Either USB or a HAT
- Speaker with AUX input or RCA
- Audio Cable
- Separeate server hosting server part of Snapcast (This is not needed but nice to have separeate device if you add multiple clients)
- Rotary encoder with 24 steps and built-in button (change volume on clients, click for pause/resume/next station)
- Breadboard for prototyping
- Wires
- Soldering kit
- Optional: button for changing station instead of clicking rotary encoder. Then resistor is needed for built-in LED.

## Docker setup for server

I usually use Docker compose for my projects. So I created a docker-compose for this.
Instructions for installing docker and docker compose, can be found on Docker's own page.

When using this project you can just use `docker compose up` for starting.
This will spin up:

- Snapcast server
- Librespot for Spotify Connect
- Shairport-Sync for Airplay
- Mopidy for Radio and local music

Snapcast has many more players, which can be read about on their Wiki in the offical repository at Github.

## Satellite rooms

Documentation about the other players can be found here: [Satellite rooms](satellite_room.md)

## Sources used for inspiration

- jessyjones @ Instructables: https://www.instructables.com/From-Record-Player-to-Multi-room-Spotify-Controler/