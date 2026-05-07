<img width="5100" height="3300" alt="Image" src="https://github.com/user-attachments/assets/e95f38e7-e53a-4ae1-bdfe-d932d8df8138" />


### **Abstract:**

Urban Restitution is a Rhino Grasshopper script designed to assist beginner architects or architects early into the design phase of the interfacing area between the building and the public realm/street. It does this by inputting some basic geometries as well as environmental conditions given by the user and returning a ranked list of “Intervention typologies” (Such as benches and Shade Trees) that would best be suited for the area as well as a simple modifiable grid upon which the best typology is placed. The system is intentionally simple and mainly meant to be used as an exploratory tool, one which can provide guidance on which ideas may be worth looking into further, rather than as a final ultimate decision maker.

### **List of Features:**


Rhino Grasshopper script that is meant for early development/beginner level designing of the interface between a building and the public realm.

Simple to use sliders for exploration of different environmental conditions and the resulting optimal intervention typologies.

Built in simple grid generator to help with intervention placement.

Required .csv has simple organization that can easily be expanded to include more typologies and environmental/site conditions.


### **Methods**

<img width="494" height="236" alt="Image" src="https://github.com/user-attachments/assets/68da37af-ce1b-467f-8add-c136e6db8f7c" />

.CSV File: Select the provided .csv file named “Urban Restitution"

<img width="309" height="386" alt="Image" src="https://github.com/user-attachments/assets/6163979f-da32-4d65-97f0-bbe6f740dd5a" />

The sliders each represent an environmental condition that is related to the site in which the user is planning around. To keep it intentionally simple the sliders are bound from -5 to 5 where the sign represents the opposite conditions and the magnitude represents how extreme the condition is.
(Example: +3 rain means that rain is more common than not, and the rain is fairly strong, whereas a -5 wind means wind is almost never present at all)

The panel beneath is the output of the ranking system, it shows the order in which each Intervention Typology placed as well as the total amount of points they acquired compared to each other.

<img width="1807" height="235" alt="Image" src="https://github.com/user-attachments/assets/a816fa72-67a8-40e8-bccb-779a79551e18" />

Manipulates the imported .csv file to a state that allows for multipliers and ranking to work.
Applies multipliers to each Intervention Typology based on the assigned environmental conditions to get final point scoring, then sorts and returns the new list.

Creates simple forms to represent the highest ranked intervention typology and applies it to a generated grid.

<img width="360" height="297" alt="Image" src="https://github.com/user-attachments/assets/28ad8d3f-0fea-4781-9b99-05b35c4b0804" />

Inputs the previously created Geometries and some grid editing sliders to generate a grid for the typologies to be placed upon.

### **Use cases:**

The two primary use cases that were envisioned for Urban Restitution are a beginner architect trying to explore how to blend a building into the greater public realm through the streetscape, or an intermediate level architect trying to find a quick starting point to do further research and designing upon.

Urban Restitution's strength is in its simplicity of use and purpose. A new designer would be able to set up the program and site in minutes and from there simply play with the sliders to explore the effectiveness of certain typologies under certain conditions. The tool in this case helps with learning as it can be used to experimentally learn what would work best for a design. 
The other case sees the Urban Restitution script be used to accelerate an already in progress project, if a designer were to feel stuck on what to do for the exterior of a building they could quickly launch Urban Restitution and in seconds be given a direction to work towards. It won't be able to make the design for them but being given a gentle push can help spark inspiration and problem solving.

### **Discussion Points:**

A major inspiration for this project is related to the homelessness issue within the United States. While I understand that a simple Grasshopper script isn’t going to solve the issue overnight, simply by making something for people to look at and recognize that our public streets have become more unfriendly to human beings I hope to inspire some subtle change in designs.

This has been an interesting project to uptake on my end as I haven’t had as much of the coding/development education as many others (being an undergrad and in a more artistic major) so much of my process was in exploration of development methods that both taught me as much as possible while keeping everything in the same space as much as possible. This is the primary reason as to why the entire script is within Rhino Grasshopper and has no Python involved. In the future as I learn more I plan on trying to streamline my script into more and more efficient programs and code but for now it functions on a basic level which is easy enough to understand and shows the logic of its function in its construction.

There are several primary roads forwards in terms of improvements to this script, the most obvious is to add more features, but another method is to add and refine the available environmental conditions and intervention typologies provided in the script.
