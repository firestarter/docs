# 🔥 Firestarter: Technical FAQ

### What is the mob cap?
We have a separate, independent mob spawn cap **per player** for the following mob types:  
* 16 hostile mobs (zombie, creeper, etc.)
* 3 animals (pig, cow, rabbit, etc.)
* 6 water animals (guardian, dolphin, squid, etc.)
* 1 water ambient (cod, salmon, etc.)
* 0 ambient (bats)

The sooner you are able to kill a mob and get it out of the cap, the faster new mobs will be able to spawn. Also note that the cap is per player, and each player has their own, independent cap (as you can see above). Vanilla has a global, server-wide cap, but this becomes a problem with a large amount of players online.

### What is the mob spawn rate?
Similar to the mob cap, the spawn rates for mobs are different for the category the mob falls under:
* Every 2 ticks for hostile mobs (vanilla: 1 tick)
* Every 400 ticks for animals (vanilla: 400 ticks)
* Every tick for water animals (vanilla: 1 tick)
* Every tick for water ambient (vanilla: 1 tick)
* Ambient mobs never tick spawning (vanilla: 1 tick)

### What is the mob spawn radius?
Mobs are able to spawn within a radius of 48 blocks (3 chunks) of the player. In vanilla, this would normally be 128 blocks (8 chunks).

### What is the render (view) distance?
We have two types of view distances on the server. While a player is able to see 7 chunks around them, only 3 chunks of that radius is considered the actual render distance. Ticking will only occur within this 3 chunk radius, and anything outside will not update unless player moves into the area.

### Why are pistons/explosions not working?
Our claims plugin prevents piston block pushing and explosions outside of claim borders, and in the case of explosions, requires **explicitly** enabling claim explosions using `/claimexplosions`. This setting has to be re-enabled after every server reboot.
