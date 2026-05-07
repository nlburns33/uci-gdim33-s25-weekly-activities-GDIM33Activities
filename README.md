# GDIM 33 In-Class Activities
## W1
### Activity 1
[Inspiration Board](https://docs.google.com/drawings/d/1tsGEH4YWukCZJdz_tZdXfr5G4T_H1BApO8bkQef3LJw/edit?usp=sharing)

1. I'm interested in shooter mechanics and more serious games as well as vehicles and military aesthetics. I also like action-focused games.
2. Jayden and I both enjoy shooter games and turn-based games. We also both enjoy competetive games.
3. There is not a lot of overlap in terms of genre apart from shooters, but we both like games that are fast-paced and require motor skills. 


### Activity 2
![33 Breakdown](https://github.com/user-attachments/assets/b8c45c94-32dd-4919-bb8b-3649a27b077b)

## W3
### Activity 1
<img width="1661" height="1093" alt="33 Breakdown Updated" src="https://github.com/user-attachments/assets/f4a33876-1d1d-41e9-99f5-80743e56dfa0" />

### Activity 2
1. It is advantageous to save the event name as a Scene variable because it makes it easy and reliable to input the name correctly. It also means that you can change the event name in the inspector without having to individually change each event. 

2. The Debug.Log() node in the transition between the Dialogue and Event states helped me to check if the transition was actually running, which actually helped because it wasn't working at first.

3. The Set Cursor Lock State is relevant to my Vertical Slice because I don't want the cursor to be present while the player is looking around.

4. The concept of a "game state" is proably not relevant as the game as a whole does not switch between specific states, but state machines in general are useful, especially for the enemy who will have multiple states.

## W4
### Activity 1

Currently, the monster and its states are present, with nearly all of the transitions working. It wanders, chases the player, and can attack and damage the player. The player can move, jump, and shoot and stun the monster.

Playtesting goal: Does the monster's behavior make sense and feel reasonable?

Team Members: Nolan Burns, Brendan Johnston, Jayden Ishibashi

Playtesting Notes: Looking around is jittery. The player can't die. The monster's behavior makes sense and correctly runs, though the stun is a bit long. The monster can also get stuck in the stun animation. The player can occasionally get stuck in the jumping state if they jump into a wall.

### Activity 2
1. A dialogue could definitely add more dialogue without writing any code. New dialogue is added via additional scriptableobjects, which can be edited via the inspector.

2. There is a limit to the number of buttons, and therefore dialogue choices, that can be on screen without adjusting the button layout, but there is no limit to how many chains of options can exist.

3. The purpose of the regenerate nodes button is to update the available nodes to include any nodes that may have been created by scripts or other methods.

<img width="1708" height="931" alt="Screenshot 2026-04-22 193521" src="https://github.com/user-attachments/assets/b1ba5ca3-ee5b-483c-afe8-cd8335f5357e" />

## W5
### Activity 1
Feature: Sanity system

Basic steps:
1. Create the sanity changing script with debug logs to test if it runs correctly
2. Have the UI correctly change with the sanity level

Detailed steps:
1. Create a new sequence in the player graph that runs on update
2. Make a new variable for sanity and have it lower by a certain amount each second when near the monster or hiding
3. Make this variable increase when the player is in a light or fully healed
4. Make a text UI element
5. Make a new sequence in the UI scripting graph that runs with a custom event. When it runs, set the meter text to the player's sanity variable
6. Create an image that 'slides' like a bar with the sanity level

### Activity 2
I implemented the sanity system so that the player's sanity lowers when they are nearby the monster or hiding in a locker. It also updates the UI whenever the sanity level updates. Picking up a medkit restores the player's sanity. 

## W6
### Activity 1
1. Sicne the last playtest, I have added ammo boxes, medkits, the hiding and sanity mechanics, created a proper scene, and fixed the jittery camera movement.
2. [Itch Link](https://nlburns33.itch.io/33-vertical-slice-playtest-2)
3. My playtesting goal is to find any bugs that might exist and whether the monster correctly switches between the different states.

Playtesting Notes:
- The monster doesn't rotate before/after attacking
- The camera clips through the player's legs when jumping
- The sanity decrease rate is too low when nearby the monster
- The player doesn't stop regaining sanity once leaving the light
- State changing works well, but the visual rotation isn't great

### Activity 2
1. The Multiply setting results in a darker and less satured color because it is multiplying two numbers less than one together, resulting in a lower number. Lower RGB values correlate with a darker and less satured color.
2. If we multiply alpha values, the result will be more transparent. The number will be lower which correlates with more transparency.
3. The shader gets the UV data from the vertices on the mesh.
4. It isn't very interesting, I already knew colors could be manipulated with math so it isn't really new information.