# in-class-activities
## Devlogs
### W1
Write your W1 activity Devlog here.
The camera doesn't follow the cat.
[itchio link](https://siyan-wu.itch.io/week1-activity)
### W2
Create future Devlog sub-headers with the three # symbols, then write your Devlogs below them.
1. Why are the r, g, and b variables floats instead of ints, bools, or strings?
Unity’s Color uses values between 0.0 and 1.0 for red, green, blue channels. Float can store decimal numbers. Int only holds whole numbers, bool is only true/false, and string stores text. So float is required for RGB color values.

2. Why is the _bounce variable an int instead of a float, bool, or string?
Bounce counts how many whole times the ball hits the wall. You cannot have partial bounces like 2.5 bounces. Int stores whole numbers, which is perfect for counting. Float is for decimals, bool is true/false, string is text.

3. The error you got after Step 4 of Part 2 told you something useful about why that line of code was broken - what was it?
The error showed a type mismatch. C# does not allow assigning a value of one data type into a variable of another incompatible type. This teaches us variables must match their data type.
[itchio link](https://siyan-wu.itch.io/w2-in-class-activities)
###W3

Activity 1
1.GetResponse
Parameters: int friendship level, bool knowsSecret
Return Type: string
The method uses friendship level and whether the player knows the secret. It returns a text response.
2. SetLightDimness
Parameter: float santyLevel
Return Type: viod
The method uses the player's sanity level to change the light brightness. It does not return anything.
3. DidPlayerHitBeat
Parameter: float pressTime
Return Type: bool
The method checks when the player presses the key. It returns true or false.

Activity 2
A class is like a coffee machine blueprint. A Component is like a real coffee machine made from the blueprint. Member variables are settings like temperature and coffee size. Methods are actions like making coffee and heating water. Different coffee machines can use the same design but have different settings.

Activity 3
The balls get extremely bright because their color is multiplied by 1.5 when they bounce at a certain speed. Every time this happens, the color values increase again. After many bounces, the values become very high, making the balls look extremely bright, especially in the Scene view. 
## Open-Source Assets
### W1
- Animals: https://assetstore.unity.com/packages/3d/characters/animals/animals-free-animated-low-poly-3d-models-260727 
- Low-poly environment: https://assetstore.unity.com/packages/3d/environments/landscapes/low-poly-simple-nature-pack-162153 


### MiniGame1 Devlog

For this project I used Unity to create a 3D platform game. To get a picture of how Unity arranges a game I think of Unity like a theater production.

Scenes are the stages. My game uses the scene as the stage where the whole game takes place. The Main scene holds the platforms, player, coins, hazards, camera, lighting and other objects needed for the game.

GameObjects are the actors and props. Every key item in the game is a GameObject. For example the PlayerCapsule is the player Platforms build the level Coins are items to collect. Hazards are obstacles that can cause the player to die.

Components are the abilities and gear of each actor or prop. A GameObject becomes useful because of the Components attached to the GameObject. For example the PlayerCapsule uses a Character Controller for movement. A Player script for the game’s player behavior. Other GameObjects use Components such as colliders so that the PlayerCapsule can interact with them. I also used scripts to control gameplay. The Player script keeps track of collected coins and points. It handles what happens when the PlayerCapsule touches a hazard. The game also has a changed player movement speed so that platforming feels different, from the setup.

Building this project helped me understand that Scenes, GameObjects and Components work together. The Scene provides the stage GameObjects provide the actors and props and Components give those GameObjects their abilities and behavior.

### MiniGame2 Devlog
Minigame 2 Devlog

One issue I had was with the chest’s health and color change. At first, the chest did not change color correctly when I hit it with a spell. I checked my code in the ColorChange script and found that I needed to fix my if statements. After changing the conditions and testing the game again, the chest changed from bright red to medium red and then dark red. The chest also disappeared when its health reached 0.

I think the line changes the color of the sprite. The period (.) is used to access something inside an object, like its color. The word “new” creates a new Color value. The “r” controls the amount of red, while 0.2f controls the green and blue values. This line helps change the chest’s color when it gets hit by a spell.
