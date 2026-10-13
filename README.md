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

## Open-Source Assets
### W1
- Animals: https://assetstore.unity.com/packages/3d/characters/animals/animals-free-animated-low-poly-3d-models-260727 
- Low-poly environment: https://assetstore.unity.com/packages/3d/environments/landscapes/low-poly-simple-nature-pack-162153 
