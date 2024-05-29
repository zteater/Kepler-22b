# Terra-Force

## Base Game
https://gx.games/games/z23hhv/terra-force

## Challenges
- Ultimate Defender
- Ultimate Defender v2
- Shield Defender
- Pure Defender

## Release Notes

### v1.0.2

Formation
- No longer forms with empty upper row
- Reduced speed increment by 50%
- Reduced drop stepy 40%
- Moved initial formation position upwards

Buffs
- Added shield buff, which has 3 hitpoints
	- Stacks with other buffs
- Added extra life buff
	- Maximum of 3 lives is possible
- Auto-fire
	- No longer persists on death

Debuffs
- Stuck
	- Changed sprite to checkboard pattern
	- No longer persists between waves
	- Now stacks duration with multiple spideweb hits

Invaders
- Mantis
	- New random spawn invader with 1 hitpoint
	- Spawns like UFO, but only 20% of time
	- On death, drops extra life or shield buffs
	- When killed last in a wave:
		- Increases shield hitpoints by 1, to maximum of 3
		- Increases buff duration by 20 seconds
- Shrimp
	- Reduced hitpoints to 1
	- Changed initial spawn wave to 5
	- Changed bomb to v-pattern bomb
- Spider
	- Increased hitpoints to 2
	- Changed initial spawn wave to 11
	- Changed bomb to spiderweb

Bombs
- Added damage points to all bombs
	- Crab - 1
	- Shrimp - 1
	- Octopus - 1
	- Spider - 0
	- Snail - 2
	- Mimic - 1
	- Squid - 2 
- Spiderweb
	- Does not cause damage to shields, but can pierce them
	
Shield
- Activated by buff from Mantis
- Initially has 3 hitpoints
- When struck by bomb, hitpoints are reduced by the damage points of the bombs
- When struck by an invader, hitpoints are reduced by invader's hitpoints

Challenge
- Ultimate Defender
	- Retired
- Ultimate Defender v2
	- New scoreboard
- Shield Defender
	- Start with a 3 hitpoint shield and survive as long as possible without losing shield
	- Players are scored based on the duration of their laser shield

Graphics
	- Fixed laser and life sprite alignment on menu
	- Fixed buff impact collisions with Terra
	- Fixed bomb impact collisions with Terra
	- Changed spiderweb to checkboard pattern
	- Changed UFO and Mimic to lighter color varients


### v1.0.1

- added snail, which drops shell mine
- changed level which aliens spawn:
	// C - Crab 1-4			
	// S - Spider 5-7		
	// O - Octopus 8-10		
	// H - Shrimp 11-13		
	// N - Snail 14-17		
	// M - Mimic 18-21		
	// Q - Squid 22		
- level difficulty now caps at level 26, speed continues to increase indefinitely
- hitting alien bombs no longer grants points
- added Pure Defender challenge, highest wave no powerups
- added buff auto-fire, hold space, does not trigger flak
- killing ufo as last invader now grants 10 seconds to existing buff
- added controls for A and D, which mirror left and right arrow

### v1.0.0

- invaders no longer shoot >800
- octopus no longer shoots at laser >750
- fixed explosion effect for shrimp bomb
- fixed uncaught exception with ocotopus bomb
- mimic now has 2 hp
- rapid fire is now a laser shot with 3 dmg
- ufo now flies low and high
- shrimp can shoot max of 2 nets at a time
