//NPC Pathing/Routine
- All routines will be dictated by the current D/M/Y and time of day.
- Each NPC will require an instance in all rooms it may appear in
- Then each time a room is entered, a check will confirm what state/position they should be in
- Paths will be determined via individual mp_grids
- Each NPC with a routine will have its own mp_grid containing all other NPCs
- Each time it enters a new cell on its grid it will check for collisions
- If one is found it will plan out a new path
- The game will essentially pause when enterting dialogue (Every object apart from dialogue partner)
- When saving the game, the grid position will be used to save the NPC path position
- When entering/exiting rooms use 1/(length/timer) to determine position

//Season/Event Changes
- A script will store triggers that will alter object variables based on time
- E.G. If it is spring fair time, the script will run on the turn of the event and populate an NPCs inventory with special items (One of kind seed?)
- Dialogue changes will be stored in individual ds_lists via their own objects, a check will confirm which list to run
- Same will apply to relationship to player e.g. if NPC has a good relationship, a more friendly dialogue list will load
- The script will also store and load world changes e.g. position of NPCs, items for events spawning, decorations etc
- Potential creature/enemy availability could also change based on season 
- As will flora/rocks/minerals/gatherables 

//Shop Behaviour
- Best to let shoppers ghost as the space in very limited
- Browse points around tables should be used as markers for movement
- More desirable items during certain times of the year will sell at a higher rate
- 
