---
name: Up You Go
tools: [Unity, C#, MediaPipe]
image: https://diogobarroso.dev/assets/UpYouGo.jpg
description: The first game I designed from scratch at Stasism
---

# Up You Go

<video controls preload="none" width="100%" poster="https://cloud.diogobarroso.dev/s/mfDQmacwb73kGnH/preview">
    <source src="https://cloud.diogobarroso.dev/s/mfDQmacwb73kGnH/download" type="video/mp4">
</video>

Up You Go was my first proposal at Stasism. After Hex <insert hex link>, I wanted to create something bigger, building on what I had learned with the first game. Taking into account the Hex primary control scheme (opening and closing your hand in front of the webcam), I had the idea of creating a climbing game. The player would use the same opening and closing hand movement to "grab" the wall piece while moving the hands to elevate the character's body and reach for another wall piece. That brought new challenges. It was demanding to move the character with this type of controls. Since the camera was already attached to the character, moving the environment according to the movement of the hands created a good illusion that it was the character who moved.

The next issue I had to solve was the leg movement. The hands moved with the players', the arms followed, but the legs were still. I learned about inverse kinematics and made the feet move from wall piece to wall piece (or pick a random point in case no wall pieces in reach are viable) to better mimic what happens in a real climbing experience. I accomplished this with a collider spanning from the hip to the foot detecting collisions with wall pieces and setting the foot's position on top of the most adequate wall piece.

After developing movement for the character, it was time to focus on the environment. The first couple of levels consisted of learning the controls and how to climb. After those, more mechanics were introduced. Falling obstacles to make the player move horizontally. Static obstacles that need a button to be pressed to move away. Moving obstacles the player needs to turn off by finding a button in the level.
