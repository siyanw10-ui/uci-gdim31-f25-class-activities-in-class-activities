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

### W3

### Activity 1

1. GetResponse

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

### Activity 2

A class is like a coffee machine blueprint. 
A Component is like a real coffee machine made from the blueprint. Member variables are settings like temperature and coffee size. Methods are actions like making coffee and heating water. Different coffee machines can use the same design but have different settings.

### Activity 3

The balls get extremely bright because their color is multiplied by 1.5 when they bounce at a certain speed. 
Every time this happens, the color values increase again. After many bounces, the values become very high, making the balls look extremely bright, especially in the Scene view. 

### W4

### Question 1

We added a Capsule Collider to the cat, a Sphere Collider to the soccer ball, and a Box Collider to the goal. We used Rigidbodies on the cat and soccer ball so they could interact with physics. We checked Is Trigger on the goal so the ball could pass through it and detect a goal. 

### Question 2

My game did not work correctly at first because I had some coding errors. I had an extra bracket and made mistakes with variable names and capitalization. I fixed these errors in SoccerBall.cs and checked my code again.


### W5

### Activity 1

Part 1: Planning

1. Member Variables

The DeerW5 class needs a public Transform variable called target and a private NavMeshAgent variable called agent. The target stores the GameObject the deer will move toward, and the agent controls its movement.

2. Methods

I used the Start() method provided by Unity. I also used GetComponent<NavMeshAgent>() to get the NavMeshAgent component.

3. Method Functions

The Start() method gets the NavMeshAgent component and uses SetDestination() to make the deer move toward the target’s position.

Part 1: Implementation

I created the DeerW5 script and attached it to the Deer GameObject. I selected Mushroom_red as the target in the Inspector. After running the game, the deer successfully moved toward the red mushroom.

Part 2: Cat Movement

Step 1

I added movement code to the CatW5 script. I used Input.GetAxis("Vertical") and Vector3.forward to control the cat with W and S. I used transform.Translate() to move the cat and Time.deltaTime to keep the movement speed consistent.

Step 2

I used an if statement and _flipWSControls to reverse the movement direction. When I checked Flip WS Controls in the Inspector, W moved the cat backward and S moved it forward.

Problems and Solutions

At first, the cat did not move because the movement code was missing. I added the code and tested it again. The cat then moved correctly. I learned how to use NavMeshAgent to move a character automatically and how to use Vector3 and keyboard input to control movement. I also learned how to reverse movement using an if statement. 


## Open-Source Assets
### W1
- Animals: https://assetstore.unity.com/packages/3d/characters/animals/animals-free-animated-low-poly-3d-models-260727 
- Low-poly environment: https://assetstore.unity.com/packages/3d/environments/landscapes/low-poly-simple-nature-pack-162153 

