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
