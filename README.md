# C346-Game
Group Project for Introduction to Software Engineering

### Team Members

* [Alan Grant](https://github.com/kurfew007)
* [Jeremy Stephens](https://github.com/sSeld)
* [Kristopher O'Bryan](https://github.com/krs24)
* [Leodan Diaz Aguilera](https://github.com/diazl2001)

[API Documentation](http://kurfew007.github.io/C346-Game/)

[Organization](https://github.com/kurfew007/C346-Game/blob/master/docs/organization.md)

[Estimations](https://github.com/kurfew007/C346-Game/blob/master/docs/estimations.md)

## What is Zombiefied?

Zombiefied is a zombie surival game. Your goal is to survive the zombie infested lands as long as possible. Throughout your journey you will encounter enemies such as hunger, thirst and of course, flesh eating zombies!

### Features
* Day based survival
* Randomized levels and procedurally generated caves
* Food and water pickups to satisify hunger and thirst
* The ability to attack and kill zombies
* Zombie loot drops

### How to Play

* Use the Left, Right, Up and Down arrow keys to navigate the playing board. 
* To attack a zombie walk towards and against the enemy until he is dead.
* You have three main attributes, *Health*, *Thirst* and *Hunger*. *Thirst* and *Hunger* will decrement over time keeping you on the lookout for any food and water drops throughout the world to replenish these attributes.
* If *Hunger* or *Thirst* reaches 0 then your *Health* will slowly start to decrement until you find the appropriate resource.
* Enemy zombies will also attack and take your *Health* away.
* When your *Hunger* and *Thirst* are above zero, you will regenerate *Health*.

## The Process

### Development
Our group agreed to develop a video game in the Unity Graphics Engine. We initially decided to design a survival game in a rogue like format with a turn based attack system. However our design changed and our game expanded to include features that are not typical of a rogue like adventure. We wanted to implement a more survival like setting in which the player must not only defend themselves against zombies but must also gather food and water to stay alive. 

### Challenges
* Unit testing within Unity was a challenge. Due to Unity handling many functions behind the scenes some processes could not be unit testing within scripts. 
* The Unity interface was new to most of us and figuring out how to navigate the interface and how it strung the scripts and assets together was a challenge. 
* We wanted to design a random cave generator that the player could explore apart from the overworld. While our generator design was successful, we were unable to successfully connect it to the rest of our game and thus this feature remains only partially complete.
* Loot drops from enemies was a tricky feature to implement. We wanted the player to be rewareded for slaying an enemy and recieve a random item drop. Our turn based movement made this difficult as the player would move to the tile of the enemy after defeating it. Whlie loot would drop the player would jump to that tile and the loot would be destroyed before the game could draw it. We were able to fix this issue by saving the tile that the player was standing on previously and simply place the enemy loot there.


