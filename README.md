# GDIM32 In Class Activities
## W1
### Activity 1
Our advice is that we should understand every code that we are writing and solve every problem that your friend (game tester) tells you.

### Activity 2
1. x=10;
2. x=2;
3. It prints "hello world" in the console every frame after the game starts.
4. MonoBehavior
5. Immediately after the game starts, print "x = 10" in the console.
6. 10 is the argument. "10" assignes the value of 10 to the parameter x. (“x = ” + x) combines a string with an int to be an entire parameter. These determines the input of the method.
7. The bug appears in the line: Transform.Translate(_direction);. Transform here is incorrect. We shouldn't use a class translate.
8. Transform should be changed into _playerTransform

### Activity 3
[MG1 break down google doc](https://docs.google.com/document/d/1RY8G4u76Aeqqu-rppdIJhAqMhHotRh3U2m445UlfjAs/edit?usp=sharing)


## W2
### Activitiy 1
![IMG_6751](https://github.com/user-attachments/assets/cd4ab5f8-9445-4936-bbcc-155ecad403ec)

### Activity 2
I created all the gameobjects required and all the scripts that will be used. I enabled the bird to stay on the ground and jump when player hits space. I finished the script of UI. I also added all necessary components I can think of so far to all the gameobjects I created so far.
[New Commit for MG2](https://github.com/UCI-GDIM32-W25/mg2-tinamengxq/commit/f14c7c1ba8b60ee409852aecf1a3c6f612339da4)

## W3
### Activity 0-2
Jingyi Bi

### Activity 3
![IMG_6784](https://github.com/user-attachments/assets/b8c913f5-4479-4f59-b932-e571aca9792c)

## W4
### Activity 0
Yuxin Ding

### Activity 1
All the rest Locators disappear after I run the game, and there is only ONE Locator left in the hierarchy. This is because of the code in the Locator. 

        if (Instance != null && Instance != this){                          
              Destroy(gameObject);                                                  
              return;                                                         
          }

This code destroies all the extra Locators in the hierarchy and make sure there is only one left running in the game. 

### Activity 2
![IMG_6804](https://github.com/user-attachments/assets/c7d76d81-a82e-482a-b793-17688d6b46a1)

### Activity 3
[Commit](https://github.com/tinamengxq/HW4/commit/34e11c850eabdac4b5424250c8e023f86b923a01)
I added sprites of bird and pipe. I sliced the sprites. I managed to arrange the scale of the screen. I added player and pipe game objects. I created player.cs. I added ground game object. I added collision component to the player and change the collider the player.

## W5
### Activity 1
I think the use of interface make it clear for me to find the responses of specific items to the same event. It makes sure that I won't forget any necessary responses of any items while compiling my scripts. I will keep it because I think that it is clear to present all the actions of each items. And also if I choose not use interfaces and abstract classes, the total amount of code will greatly increase.

### Activity 2
in the second demo, what classes represent the Model, View, and Controller aspects of the MVC pattern used in the scene?
Model: Item.cs, Enemystats.cs
View: DialogueBubble.cs, Inventory.cs
Controller: Enemy.cs, Player.cs

### Activity 3
#### Scenario 1
scriptableobjects: each button (sprites, _movespeed)
finite state machine: player whether missed button & different scores each button will give
model-view-controller:
    - model: list of buttons(buttons)
    - view: score UI, time count down
    - controller: response to player's finger, 
singleton: locator of player
inheritance: button move to a place, button disappear and add scores. 
#### Scenario 2
model-view-controller: 
controller: the ability to causing damange to other players
view: ui that activate the ability
finite state machine: different arms cause different harms & player's living state
#### Scenario 3
finite state machine: plants' growing status
model-view-controller: 
controller: ability plants grow
scriptableobjects: different plants

### Activity 4
Attendance: Tina Meng, Yuxin Ding, Yan Zhang
[Final draft proposal](https://docs.google.com/document/d/1oGQXyqTOWLLG3tDOO_RGtfLVnASe5ZuaAI4uGt-2Nhs/edit?usp=sharing)

## W6
### Activity 1
- Gizmos:
    1. The animal and the fruit change the directions that they face while moving. 
    2. Gizmos function helped create a red line to show which direction they two gameObjects are facing. 
    3. I want to track which direction the player is facing in the final project. I also want to track the direction that the NPCs are facing. Thus, I can try to make NPCs look at the player in the game. Gizmos may help me to find the certain directions. 
- Breakpoint
    1. Prof created a breakpoint at the code CapybaraW6Demo3.Instance.ResetLocation(); This calls the singleton
    2. This breakpoint stops unity. We can debug without writing the debug lines, which will take longer time. 
    3. CALL STACK, to see what chain of events happened before the breakpoint works
    4. It would be useful to debug when coding the final project.
- Profiling
    1. Modifying the movement of prefab. 
    2. Using only one Gizmos function to govern all the prefabs.
    3. No idea how to use it in the final project. But I think I will definitely use these because the final project must be very large as there are many assets and classes. The game might run very slow. 

### Activity 2
Attendance: Tina Meng, Yan Zhang, Yuxin Ding
[Final proposal draft](https://docs.google.com/document/d/1oGQXyqTOWLLG3tDOO_RGtfLVnASe5ZuaAI4uGt-2Nhs/edit?usp=sharing)

## W7
### Activity 1
1. when the gizmos red line goes through an object in the environment, a red sphere will appear on the object to show the "passing through"
2. Raycast only returns true/false. False: the line didn't hit anything; True: did hit sth., then check the point the line hit.
3. Spherecast is looking at an area containing the sphere instead of looking at an ray to so if there are sth. in the way. (Might be a better choice than raycast)
4. If we use Debug.Log(), matrixes will be presented in the console. 

### Activity 2
Attendance: Tina Meng, Yuxin Ding, Yan Zhang

### Activity 3
