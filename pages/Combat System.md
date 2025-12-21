## Overview
- Nebu is a stat based combat system, so I will start by laying out the different combat stats that you should know
- ### HP (Health)
	- Your health. The base value for this is 100, and it can be raised through the [[Durability]] stat and its related perks. Health does not naturally regenerate.
- ### Charge
	- The energy that you need to use skills. The base value for charge is 5, and it can be raised through the [[Charge]] stat and its related perks. 1 energy is regenerated per turn by default.
- ### Speed
	- Speed determines when you (and your team) get to attack. Having a high enough speed allows for you to perform additional actions while in combat, and speed can be raised through the [[Agility]] stat.
- # Combat Sample
  collapsed:: true
	- Combat in Nebu is broken down into two states, which are the attacking state and the defending state. For the sake of the explanation, I will be describing a 2v2 battle between 4 NPCS while explaining the combat system.
	- To keep it simple, all 4 NPCS will have the base 100 health and no perks or stat point bonuses.
	- ## Part 1: Speed
	  collapsed:: true
		- To start the battle, all 4 NPCS roll for their speed values. The default roll for this value is a 1d20, but this can be altered by either perks or status effects. I will be using the default dice value (1d20) for all 4 NPCS here
		- Hero 1 rolled 19
		  Hero 2 rolled 8
		  Villain 1 rolled a 16
		  Villain 2 rolled a 3
		- Because hero 1 has the highest roll among all participating combatants, the hero team will be the first to attack.
		- This step is only done once at the beginning of a combat encounter
	- ## Part 2: Attacking State
	  collapsed:: true
		- Since a member of the hero team had the highest overall speed roll, they will be the first to enter the attacking state. While in the attacking state, the hero team can choose to use any of their abilities to freely attack the villain team.
		- In the attacking state, the attacks will be declared first for one side, then the defending side will follow up with their own defensive skills.
		- Hero 1 rolls a 18 to attack Villain 1
		  Hero 2 rolls a 8 to attack Villain 2
		  Villain 1 rolls a 10 to block and takes 8 damage (To get this value, subtract the attack roll from the block roll. 18-10=8, so villain 1 takes)
		-
	- ## Part 3: Applying Status
	  collapsed:: true
		- After the hero team used their attacks, it is now time to apply status effects. As players, you all don't need to worry about this since the DM will handle this part for you, but knowing how to apply status effects can be very beneficial, so make sure you read up and know how to kill the enemy better!
		- Villain 1 is inflicted with Bleeding(1)
		  Villain 2 is inflicted with Bleeding(2)
	- ## Part 4: Defending State
	  collapsed:: true
		- Now it is the villains turn to attack. After the villain team chooses which attacks to use, the hero team can decide how they want to attempt to defend from the attacks.
		- Villain 1 is using Evil Drain with a roll of 16 aimed at Hero 1
		  Villain 1 is using Wicked Blow with a roll of 12 aimed at Hero 2
		  Villain 2 is using Cinderblock with a roll of 6 aimed at Hero 2
		- Since there is only one attack aimed at Hero 1, the option for them is simple, and they choose to block the attack. However, its a little more complicated for Hero 2. Since there are two attacks aimed at Hero 2, they have to choose to take the damage of one of them since they cannot block or evade two attacks at once. In this case, Hero 2 chooses to block Wicked Blow and take the damage from Cinderblock.
		- Hero 1 rolls a 12 and takes 4 damage
		  Hero 2 rolls a 16 and takes 1 damage + 6 from Cinderblock
		- Now that the defending state has ended, status effects are applied to the Hero team. Since Hero 2 took more then 5% of their HP as blunt damage from Cinderblock, they are inflicted with Dazed.
		- Hero 2 is inflicted with Dazed(1)
	- ## Part 5: Turn End
	  collapsed:: true
		- Now that both teams have taken their attacks, the turn ends. Any status effects are procced here, and all regen effects are applied. Regen effects and positive status effects take priority over negative status effects
		- Hero 1 heals 5 HP (96->100)
		  Hero 2 heals 5 HP (93->98)
		  [Dazed] Hero 2 loses 2 AV (8->6)
		  Villain 1 heals 5 HP (92->97)
		  [Bleeding] Villain 1 loses 1 HP (97->96)
		  Villain 2 heals 5 HP (67->72)
		  [Bleeding] Villain 2 loses 3 HP (72->69)
		- Now that the turn has ended, the cycle repeats!