## GAME_PROGRAM-EX--7


## AIM :
To implement-chasing when AI see the player.

## ALGORITHM :
STEP-1: Set up the AI character Blueprint and add a Sphere Collision component to the AI character Blueprint and position and scale the Sphere Collision component to represent theAI's detection range.

STEP-2: Create a new AI controller Blueprint and select Create Basic Asset > Blueprint Classfrom that choose the AIController as the parent class.

STEP-3: Open the AIController Blueprint and drag off the execution line and search for "Set Sight Radius" where the Sight Radius value to the desired range for the AI's vision.

STEP-4: Implement perception for the AI and connect the output of the AI Perception Component node to the AI Controller's .AI Perception property in the AI Perception Component node, configure the settings for sight and sight sense

STEP-5: Implement the chase behaviour if the stimulus is the player character, drag off the execution line and search for "Move To Actor" and set the Move To Actor node's target to the player character.

STEP-6: Create blackboard keys for the AI and create a new blackboard object and assign it to the AIController's Blackboard property. Drag off the execution line again and search for "Create Blackboard Key".

STEP-7: Update blackboard values. Set the Blackboard Key to the "PlayerLocation" key youcreated earlier.

STEP-8: Set up the Behavior Tree by Open the Behavior Tree asset in the Behavior Tree editor. Drag and drop a "Blackboard Key Selector" node onto the grap.

## OUTPUT :


<img width="1138" height="581" alt="Screenshot 2025-11-14 002939" src="https://github.com/user-attachments/assets/9d8f3ac1-3da0-4235-839a-efcdbb065b9e" />


<img width="1138" height="472" alt="image" src="https://github.com/user-attachments/assets/206fcb9c-b968-460d-ba7f-bb2d1aebaf61" />


<img width="1122" height="426" alt="image" src="https://github.com/user-attachments/assets/d2640d8a-fe74-4f95-bf11-5c770466b3a1" />


## RESULT :

Thus, the AI concept to the actor for a random movement is implemented.


