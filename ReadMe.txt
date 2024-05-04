<<--------------------------------------------------------------------------------Graphics_Project_01---------------------------------------------------------------------------------------------------------->>
# Developers

	- This project was done by Max Sherwin

# About Project
	
	- The project reads the scene contents( i.e the model properties, position, light properties, position etc) from the json file located in "GraphicsProject->DummyMain->SceneDescription.json". The project loads the models and the light settings as mentioned in the human readable file and displays a sensible scene. 

	- In my scene I have created a world where in a fantasy world, the soldiers are powerless against the ancient creatures, Beholders. Crystals grow in an irregular pattern all around and they glow at night. The scene description goes like this : The Beholder stands tall as all of the soldiers lie death under it. The Beholder charges it's final "eye-beam" to eliminate the last wounded soldier and at the last moment, reinforcement(A transport ship model that I found) arrives with it's searchlights, searching for the soldiers.

	- The scene projects various models such as trees, grass, tree base, etc to give out a forest look. And since the scene happens in the night, there are crystals around the forest that illuminate the forest to some extent, but not too much. To visual this scene effectively, the user has been given camera controls to easily move around and view the scene however the user desires.
	
	- Also except the dead soldiers everything else look colored in the scene. That's because the Beholder kills them and drains them off their life energy. So this takes away their colors in this fantasy world. I have used Meshlab to add colors and also changed the colors on the json file for the other objects. SO it's not that I wasnt able to color them, but just leaving them as such just to capture the storyline :)  
	- The json file holds the scene description and changing the json file will change the scene. But the format of the json file should be the same to load the scene. 

## How to build and run : 
	- The solution "Graphics_Project_01.sln" has to be built(either in debug or release platform mode) and then once succeeded(probably will!), make the "ReadSceneFromJson" project as the startup project and now it'll be able to run for some visual treat. 
	
### Controls :
	- Default Controls : There are a few controls that I've added :
		- W, A, S, D, Q, E = Move camera Front, Back, Left, Right, Up and Down respectively. 
		- Mouse movement = Camera can be rotated using the mouse
		- Spacebar = Spacebar pauses and resumes the mouse movement, if the user thinks the cam rotation is in the way of examining the scene(By default the cam rotation is in a pause, so when the scene 			loads, press Spacebar to activate camera rotation using mouse)
		-  1, 2, 3, 4 = These numbers keys can be pressed to showcase 4 different angles of the scene.

	- Extra Controls : There a few controls that enable the user to manipulate the models in the scene :
		- CTRL + W, A, S, D, Q, E = To move the models around, Front, Back, Left, Right, Up and Down respectively.
		- CTRL + C, V = To scale the model down or up respectively.
		- CTRL + Z, X = Shift to previous model or next model respectively.
		- CTRL + B = Turn on/off wireframe mode for the selected model.

#### Limitations to the project : 
	- Although the mouse camera rotation is a bit effective than the keypad, it's still not perfected. There are some flaws like, when the mouse movement is paused and resuming the mouse movement after moving the cam position, the rotation seems to be irregular at first and then gets used to the new perspective. 
	- Rotation in code works to some extent but not entirely, I need to look deep into the rotation code or change the whole matrix/vertex multiplication to make a proper model rotation. Right now, it's not perfected.    