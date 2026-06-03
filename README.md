# GAME_PROGRAM-EX--2
# EXP - 2 Create a player movement using character, collectable, player health and score 
### Name: PRIYADHARSHINI J
### Reg no : 212224230210

## Aim

To design and implement a simple game in Unreal Engine using a playable character with movement controls, collectible objects for score increment, player health management using traps, and level transition based on score and health conditions.

## Procedure
1. Create the Project
   
Open Unreal Engine and create a Third Person Project.

Use the default Third Person Character as the player.

Create a basic level using cubes, walls, and ramps.

3. Implement Player Movement

Use the default Third Person Character blueprint.

Configure keyboard inputs:

W – Move Forward

S – Move Backward

A – Move Left

D – Move Right

Space – Jump

Test the movement in Play Mode.

4. Create Collectable Coins

Create a new Actor Blueprint named Coin.

Add:

Static Mesh (Coin model)

Sphere Collision

Create a variable Score in the Character Blueprint.

In the Coin Blueprint:

Detect overlap with the player.

Increase Score by 10.

Destroy the coin after collection.

Add a condition:

If Score ≥ 100, load the SuccessMap level.

5. Create Player Health System

Add a variable PlayerHealth in the Character Blueprint.

Set the default health value to 1.0.

Create a Trap Blueprint named PlayerTrapper.

Add:

Static Mesh

Box Collision

On player overlap:

Reduce PlayerHealth by 0.1.

Update the health bar.

Add a condition:

If PlayerHealth ≤ 0, open the GameOverMap level.

6. Create User Interface (UI)

Create a Widget Blueprint named PlayerUI.

Add:

Progress Bar (Health)

Text Block (Score)

Bind:

Progress Bar Percent → PlayerHealth

Text → Score

Add the widget to the viewport when the game starts.

7. Testing

Play the game.

Move the character around the level.

Collect coins and verify score updates.

Enter trap areas and verify health reduction.

Confirm:

Success screen appears at Score = 100.

Game Over screen appears when Health = 0.

# Output:
<img width="1919" height="1125" alt="image" src="https://github.com/user-attachments/assets/70627ea5-e376-43a9-9494-56bf5faf8294" />
<img width="1919" height="1050" alt="image" src="https://github.com/user-attachments/assets/a846af7e-9bc4-4054-8b3a-4d2e52bc2eb9" />

<img width="1919" height="1038" alt="image" src="https://github.com/user-attachments/assets/7d3c3ea4-7681-4ecf-8450-fafc77e0e34f" />
<img width="1911" height="1039" alt="image" src="https://github.com/user-attachments/assets/716cc1b8-d702-4f62-8183-823fd7b4d679" />
<img width="1919" height="1048" alt="image" src="https://github.com/user-attachments/assets/aaa57b6e-d690-4502-bfc2-4db7db789d5c" />

# RESULT
The AI character successfully roams within the defined NavMesh area, choosing random destinations at intervals using the Behavior Tree logic.

