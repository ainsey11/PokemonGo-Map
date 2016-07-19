<p align="center">
<img src="https://raw.githubusercontent.com/AHAAAAAAA/PokemonGo-Map/master/static/cover.png">
</p>

# PokemonGo Map

[![Build Status](https://travis-ci.org/AHAAAAAAA/PokemonGo-Map.svg?branch=master)](https://travis-ci.org/AHAAAAAAA/PokemonGo-Map) [![Coverage Status](https://coveralls.io/repos/github/AHAAAAAAA/PokemonGo-Map/badge.svg?branch=master)](https://coveralls.io/github/AHAAAAAAA/PokemonGo-Map?branch=master)

Live visualization of all the pokemon (with option to show gyms and pokestops) in your area. This is a proof of concept that we can load all the pokemon visible nearby given a location. Currently runs on a Flask server displaying a Google Maps with markers on it.

Building off [Mila432](https://github.com/Mila432/Pokemon_Go_API)'s PokemonGo API, [tejado's additions](https://github.com/tejado/pokemongo-api-demo), [leegao's additions](https://github.com/leegao/pokemongo-api-demo/tree/simulation) and [Flask-GoogleMaps](https://github.com/rochacbruno/Flask-GoogleMaps).

------------

#Basic Installation Guide

On your server, install python, python-pip and github. you may wish to install screen too.
clone this repo and cd into it
run sudo pip install -r requirements.txt

once all the requirements are installed, go to the credentials.json file and change the final line to your google maps javascript api key
 to run the server run the following command :
screen ./example.py -H <ip to bind to (use 0.0.0.0 for all ifaces)>  -P <port number> -u <pokemon go username> -p <pokemon go password> -l "<postcode>, UK" -st <steps (mine was at 5>
