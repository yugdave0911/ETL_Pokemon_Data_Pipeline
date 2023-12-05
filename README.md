# ETL_Pokemon_Data_Pipeline

## Introduction

Growing up, *Pokémon* was among the favourite animated series of many ‘GenZs’, including ours. The craze for *Pokémon* trading cards was at the peak, which basically had details about different species. With this project, we aimed to recreate those experiences by developing a comprehensive database for *Pokémon* statistics. By amalgamating and organizing diverse datasets encompassing *Pokémon* characteristics, evolutions, debut episodes, and more, our aim is to unlock a treasure trove of insights and applications. The world of *Pokémon* is vast and diverse and we believe that our project is a small step towards the voyage into the heart of *Pokémon* analytics. We've incorporated analysis and visualization to explore potential enhancements for this project.
The main goals of our Data set analysis could be one of the following:
• Pokemon abilities and power analysis: Game developers and players can analyse different
pokemons to find about over powered or under powered Pokemons and develop their
strategies based on that\
• General information about Pokemons: Our analyses can be used for knowing fun facts
about Pokemon.
• Develop classification models: Machine learning and Data Scientist engineers can use our
database for practicing to develop classification models for different pokemons based on
their classification on : Legendary, generation, HP, Attack etc

After scouting the web from the myriad of *Pokémon* datasets available, I gathered three primary datasets from two datasources, which fit perfectly for the scope of this project. The datasets are as followed:

1. Pokemon Dataset: A comprehensive list of around 800 Pokemon from [Kaggle.com](http://Kaggle.com) which was compiled from various sources. It contains Pokemon name, Japanese name and other important statistics - https://www.kaggle.com/datasets/rounakbanik/pokemon, originally scraped from http://serebii.net/

2. Pokemon dataset with Evolution details: A list of around 1500 Pokemon with more statistics and also details on evolution which is one of the most important part of this project. It is also taken from [Kaggle.com](http://Kaggle.com) - https://www.kaggle.com/datasets/mrdew25/pokemon-database 

3. Pokemon debut episodes - A list of debut episodes for Pokemon from the animated series. It was taken from [Bulbapedia.net](http://Bulbapedia.net) and converted to CSV using the online tool - [https://bulbapedia.bulbagarden.net/wiki/List_of_Pokémon_by_anime_debut](https://bulbapedia.bulbagarden.net/wiki/List_of_Pok%C3%A9mon_by_anime_debut) 


## Database Design

### ER Diagram

## Workflow diagram

![Workflow_diagram](https://github.com/yugdave0911/ETL_Pokemon_Data_Pipeline/assets/96373480/beb9b24b-1bee-424b-a4a2-5949dda8f810)





## Loading Data into my Database

- Inserting data using the pokemon_episodes.csv file
- Since all our csv files have different number of Pokemon, we have inserted data into the main pokemons table merging all of the data available and avoiding duplicates
- The idea behind selecting the pokemon_debut.csv file first is that it is the only file which provides a connection between a Pokemon and its' debut episode which would be lost if we only inserted episode details using this file



## Visualisation

- We used SQL and Matplotlib to visualise some patterns in the database we created
1. How many Pokemon evolve by ‘Levelling Up’ as opposed to ‘Other’ methods?


![output_16_0](https://github.com/yugdave0911/ETL_Pokemon_Data_Pipeline/assets/96373480/b1a190c8-c0ab-4794-94a1-5d854e435bb0)

2. How many Pokemon are for each ‘type1’?
Each Pokemon has either one or two types based upon the species. These 'types' help us identify the strengths and weaknesses of a Pokemon over another type and would be critical in deciding the overall result of the duel among other factors. For example, A 'Water' type Pokemon will be pitted against a 'Fire' type Pokemon. There are a total of 18 types in the Pokemon universe
![output_18_0](https://github.com/yugdave0911/ETL_Pokemon_Data_Pipeline/assets/96373480/f0d04b5c-7fc2-4f8b-af80-ad64871787f2)




