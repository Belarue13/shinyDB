# shinyDB
Program to calculate shiny odds in pokemon games based on location and previous encounters. All data must be user generated. I only added pokemon ruby and sapphire Fiery Path.

**REQUIRES JDK 20+ AND WINDOWS**

Note: when prompted to enter a game name, if the txt doesnt exist for it yet, one will be made for you when you add to database.

[p] - calculate the odds of encountering a pokemon at a location + its shiny rate or find all locations and odds of a pokemon.
[l] - calculate the odds of encountering every pokemon at a location and their shiny rates.
[e] - calculate the odds of encountering a shiny after already encountering non shiny varients.
[a] - add a pokemon to the database. Requires pokemon name, location, and encounter rate.
[c] - close program


//notes:
Math works when using shiny charm

Some potential issues you may run into:
if you search for a pokemon like Mew, and you have both Mew and MewTwo in the same location, it will print MewTwo's data if it is above Mew in the dataset.
example:
Try to find Mew's data in route 6:
MewTwo [route 6] 50
Mew [route 6] 20
prints data for MewTwo instead of Mew.

A similar issue is with location names and pokemon names, should never encounter this issue, but its possible. 
example:
Try to find route's data in route 6:
machop [route 6] 50
route [route 6] 10
prints data for machop on route 6. Obviously there isnt a pokemon named route, but maybe there's a location that contains the name of a pokemon idk.
