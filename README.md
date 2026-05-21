# GDIM 33 In-Class Activities
## Wk 1
### Activity 1
Mood board: 
[Link](https://docs.google.com/drawings/d/1FzHw0snFg2F6ypzWUP6gd9ILTZMrTsw-iBYU8GAcVxg/edit?usp=sharing)
<img width="960" height="720" alt="Joshua Paxton Devlog Mood Board" src="https://github.com/user-attachments/assets/beb1b261-a02e-4574-9fa0-e6af0cdd227d" />

1. There aren't too many patterns emerging from my drawing board. Mainly, the pattern I see is that I like character designs with lots of lore behind them, which can go along with my appreciation of abstract album covers to create character designs that are abstract in their design, but that abstractness works towards creating a design that incorporates that lore into it. I'm not an artist myself, but I hope I could incorporate that into my design.
2. My tablemate had a style board more focused on cars, which isn't in relation to my board, but I do also like cars a lot. I just didn't want to incorporate that on my inspiration board.
3. My LA liked Overwatch as well, which I inquired to him about what characters he liked playing in the game. He said he liked to play DPS heroes, but didn't specify on which was his favorite to play. It seems he also really likes hero shooters and likes the lore behind the characters.

### Activity 2
Basic 2D Mega Man-like idea:
[Link](https://docs.google.com/drawings/d/16qWkAFiQ3Pfj0BlwnqwOK9GG7Tn62i4i53KH2tp2r0g/edit?usp=sharing)
<img width="960" height="720" alt="Basic 2D Mega Man-like platformer breakdown_Joshua Paxton-4" src="https://github.com/user-attachments/assets/0341fe07-ab6d-4517-beb1-202fe11b4d69" />

## W2
Write your W2 Devlog here.

Continue adding additional headers below this one for future weeks and future activities.

## W3
### Activity 1
Updated Break-Down: 
<img width="960" height="720" alt="Basic 2D Mega Man-like platformer breakdown_Joshua Paxton-5" src="https://github.com/user-attachments/assets/8ae87090-2b0a-4631-a473-9fba1031a55f" />


### Activity 2
1. It is advantageous to save the event name for the explore-to-dialogue state transitions as scene variable because that allows it to be used across all scripts in the scene, which will save its state between scripts and allows it to be called again with no difficulties.
2. Using a debug log node helped me when I was trying to get the state transition from the explore state to the dialogue state to work. Whenever I clicked, the dialogue wasn't opening, but with a debug log node, I could see that my clicks were registering, which meant that the issue was dealing with the node after the debug node. From that point, I was able to figure out how to fix it.
3. The set cursor lock state isn't relevant to my vertical slice, as all of my controls are meant to be used with keyboard controls as opposed to mouse inputs, so the state of my cursor doesn't matter.
4. I will be using a game state in my vertical slice. Most likely, it will be used to play animations, such as if the player is damaged, switch the player model to a damaged sprite for half a second.

## W4
### Activity 1
Playtest build: https://phazon-xr20.itch.io/cybershift-first-build
Playtest partners: Jasmine & Gio

I have the basic movement mechanics working in my build, alongside shooting, although the player can collide with their own bullets. I also have a small section of the tilemap created. 

My main goal in this playtesting is to see how people like the aestetic of the game currently, because I already know I have a lot more to do in terms of further coding the gameplay.

Playtesting notes: I need to edit my box collider on my player since it includes my gun asset, which keeps getting stuck on the edges of my tilemap. I also need to edit the parallax effect on my background, since the background elements are moving too fast to where it either looks like my player is moving too fast, or the background is glitching out. I also should remove the collison of my projectiles that I shoot, which I already knew to do. However, they really did like the scrolling background I created.

### Activity 2
1. A writer could add more dialogue to this setup if they understand the visual scripting logic behind it. All they really need to do is add more ScriptableObjects with dialogue onto them. However, if they wanted to add more than options, they would need to know how to code in the ability to add more options.
2. There is a limit of 4 dialogue options that can be added without adding any more code.
3. The regenerate nodes button allows Unity to add in any additional variables and events that were created in C# code that weren't present when the nodes were originally created. This will allow the new variables and events to be added as nodes with the old nodes.

## W5
### Activity 1
I've integrated tilemaps as platforms already, but my goal today is to learn how to use tilemaps to paint and instantiate enemies as interactable game objects across my level. I don't know how to paint game objects with tilemaps, but it will be very useful in filling out my level once I learn how to do it. 

Proposed Steps:
1. Convert an enemy sprite(s) into a usable sprite sheet by changing the sprite mode and slicing it.
2. Potentially combine sprites into a sprite sheet if they cannot be used individually
3. **Figure out how to use the game object brush**
4. Assign the created sprite sheet to the enemy prefab
5. Paint clones of the enemy prefab around the map on usable objects
6. Potentially use a debug log to test the clones for collision with my already created projectiles (they won't deal damage yet)
7. Profit 🤑

### Activity 2
Doumentation I used to create this: https://docs.unity3d.com/Packages/com.unity.2d.tilemap.extras@8.0/manual/GameObjectBrush.html

In class, I was able to figure out out to use the game object brush to paint my enemy objects on my game's canvas. It was hard trying to do this, because there isn't much documentation, and a lot of the LA's hadn't used this specific aspect of tilemaps, but after a lot of perseverence and asking for help, I was able to figure it out. Now, I will use this to paint my enemy objects across my game level so I don't have to copy and paste copies of them across the whole level.

## Wks 6-7 were excused 

## W8
### Activity 1

From my last playtest build, I have made my enemies interactiable in terms of the player taking damage from them, and the player being able to deal damage to them. I have also created a boss enemy at the end of the level that cycles through 3 states: an idle state, a jumping state, and a shooting state. I also made the charge shot ability into an actual power up. which can be found near the middle of the level and allows the player to hold down the shoot button for a second and a half to release a charged up shot that deals triple damage to enemies. 

My playtesting goals are to basically show off what I currently have so far to see people's opinions on them. I already know what I still need to do, but I just haven't had the time to do it for this build. Really, I just want to see people's reactions of what I was able to make in the limited time I had.

People who playtested: Gio and Angel

Notes: The platforming gameplay is solid, but I need to flesh out the responsiveness of the combat. I should add a little flash when enemies are taking damage and when the player takes damage. I should also add a little flash when the player is charging up the charge shot for clarity's sake. I might also add in a little dialogue when the player picks up the power up just so they know more clearly what it is they got. I should also work on the tilemap side hitboxes so the player cannot stick to them when they run into them while jumping.

Build link: https://phazon-xr20.itch.io/cybershift-may-20th-playtest-build

### Activity 2c

1. The name of the effect we created in the frame debugger is FullScreenPassRendererFeature. We can tell because when we highlight it in the frame debugger, it applies the metallic texture to the screen.
2. At a lerp value of 0.5, the screen has a faded imprint of the metallic texture, while still retaining most of the green background color it had before. At 0, it has no metallic texture at all, and at 1, the whole screen becomes full of the metallic texture effect.
3. The screen looks like this at the different lerp values because the lerp value is multiplying the two texture values, which gives the “percentage” value that is displayed on the screen, which determines how much the two effects are fused together on the screen.
4. We use (sin(time)+1)/2 as the lerp value to fix the issue because (sin(time)+1)/2 is the proper oscillating sine wave formula, which will properly go through the values from 0 to 1. Just using sin(time) won’t properly oscillate, which leads to the bright stage that wasn’t supposed to happen.
