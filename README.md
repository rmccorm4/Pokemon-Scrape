# Pokefetch
This is a script I'm working on to further my webscraping skills
## Tools
Python 3
* Requests
* BeautifulSoup

Bash
* catimg

[Serebii](https://www.serebii.net)
* Currently rewriting my scraper to use [Bulbapedia](http://bulbapedia.bulbagarden.net)

## Context
This script currently asks for the pokedex number of the pokemon you'd like
to get information about, then it will get the picture and some related
information such as type, abilities, weaknesses, etc.

I wanted to model the output to be similar to screenfetch and neofetch, two popular scripts to grab system information.

![Alt text](imgs/neofetch.png?raw=true "Neofetch Example")



## Setup

### Starting steps:

Clone this repository to a directory of your choice in the command-line:
```
git clone https://github.com/rmccorm4/pokefetch
```

Make sure you have all of the necessary third-party libraries described below

#### Python requests module 

```
pip install requests
```

#### Python BeautifulSoup module 

```
pip install bs4
```


#### catimg

On Arch Linux:
```
yaourt -S catimg
```

Otherwise, follow the instructions here:
[https://github.com/posva/catimg](https://github.com/posva/catimg)

### Disclaimers

The "Gender" category that gets printed out uses ascii symbols and may
not print properly depending on your terminal configurations. 

Personally, I use `adobe-source-code-pro-fonts` and I make sure that my 
terminal's default encoding is `UTF-8`

### Running the script:

```
./pokefetch.sh <pokemon_name>
```

Example below.


## Current progress
This is what I have so far:

![Alt text](imgs/progress.png?raw=true "Pokefetch Example")

However this requires a full-screen terminal in order to come out nicely.

## To-do

* [ ] Make sure it works for every single pokemon, including difficult names such as "Mr. Mime" and "Ho-oh"
* [ ] Get higher quality images to output if possible, need to research this more
* [ ] Conversely, try to find more pixellated versions of the newer models in hopes of getting a prettier output
* [ ] Add a -shiny flag to output the shiny sprite instead of the regular one
* [ ] Scrape more relevant information about the pokemon
* [ ] Make script work for default size terminal as well as full-screen?
* [ ] Rewrite my scraping method to be much cleaner and more uniform
* [ ] Include Gen VII pokemon
* [ ] Implement old-school sprites because they come out much nicer as seen below
* [ ] Possibly add old school gifs from the special games like yellow and crystal

![Alt text](imgs/oldschool_sprite.png?raw=true "Old School Sprite Example")
