CONTROLS:
left click for use
wasd for movement
space for jump
shift for sprint
control for crouch
tab for inventory
e for interact
r for reload
number keys 1 to 6 for hotbar use

NOTE: the gun currently lacks a reloading animation, so when there are no bullets loaded yet (e.g. at the start of the game), pressing reload or firing would reload the gun, where you have to wait a short momenent before you can shoot. This is intentional and is not a bug.



fpsmovement version 2:
added inventory system

Inventory:
there is a hotbar that is always visible, pressing the number keys would use any consumables that are in it (note: only the heal potion is considered a consumable)
clicking on tab frees the cursor and allows you to interact with the full inventory. 
-click on any item in the inventory to pick it up, click on another one to either stack it (only if the item is stackable, i.e. apples, heal potions, books, and also it does not exceed the max stack number, 99) or to replace it with the one in the slot (i.e. pick up the other one instead)
-right clicking with a stackable item that has more than 1 singular one in hand onto another slot will place 1 of those items into the slot, which can be stacked
-items in the inventory can be moved around and stacked as needed (except for the unstackable ones, i.e. the book)
-clicking on any space outside the inventory with an item in hand will drop the item, right clicking will drop only 1 of the items, these items would be available for pick up
-there is an extra slot on the right of the main inventory that can store 1 "equip" item, i.e. the helmet
-any items in hand will be dropped upon closing the inventory

Item Pickup:
-there is an apple that falls onto the brown block, that serves as an example of an item that could be given in the game. 
-the items (if stackable) will stack with another stack of the same item in the inventory (if it doesn't exceed the max stack limit)
-should the item not be able to stack, it will instead be placed in the first available slot

Consumables:
-as mentioned above, consumables (i.e. the heal potion) can be used either by pressing numbers in the hotbar or right clicking on it whilst it is in the inventory (not in hand)
-the item will decriment by 1, and it will do its intended effect (there is a health stat that is increased when using the heal potion, but is not shown yet)

Chest:
-the green block that is on the platform is a chest, which you can interact with by pressing "e" whilst you are within the range
-the chest inventory will appear, and you can drag items between your inventory and the chest one freely, with the same rules that apply
-closing the chest inventory saves the items, if any, left in the chest
-moving too far away from the chest with the chest inventory open will force close it



fpsmovement3:
added a weapon and damage system

Inventory:
there is a a newly added weapon slot below the equip slot that allows the placement of a weapon (i.e. the pistol)
-placing a weapon in the slot will show its corresponding mesh and also allow for you to use it

Weapon:
the selected weapon can be used by left clicking
-the current weapon, a pistol, can deal 1 damage per shot
-the weapon system works by casting a ray from the camera, not the weapon itself, so it will always hit directly at the crosshair
-there is a range limit set on the weapon, currently 10 for the pistol

Enemy:
the enemy is another capsule:
-it has a max health of 10, so can survive 10 shots from the pistol before dissappearing
-this enemy is universal, uses resources to load so it can take on any shape and any health or defense as needed

Plans for update 3.1:
-addd a projectile for the weapon when shooting
-add reload and a max load limit to the weapon
-add consumable bullets to inventory and consume when used

fpsmovement3.1:
Weapon:
added recoil
-also added sfx when firing, and a bullet hole where hit
-some visual and performance changes

Inventory: 
added bullet consumables
-there are now different bullet types for different weapons

fpsmovement4:
World:
-added some obstacles for testing
-enabled navigation mesh

Bots:
-the "enemies" can now move on their own, and will move randomly along the navigation network until it sees the player
-it will then shoot at the player, until the player is no longer visible
-there is an accuracy meter that can be set
-uses the same visuals as the player
-detects when the player is hit, but there is no health system yet, so it only prints "hit player" currently

fpsmovement5:
World:
-combined with maze
-randomly spawns some enemies after the previous ones have died

Weapon:
-some visual improvements
-added bobbing and idling and swaying

Player: 
-added crouching


