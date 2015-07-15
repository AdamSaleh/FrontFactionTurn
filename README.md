# Front Faction turn

A GM tool to formalize different NPC factions working on interfering fronts.
Conceptually, GM would make sure, that after a certain in-game time, each faction
had chance to roll to advance their agenda, in adition to interfering with agendas of other factions.

# Basic rules

I took most of the dice rolling from yet unreleased (Blades in the Dark)[https://www.kickstarter.com/projects/2080350433/blades-in-the-dark].

## Faction turn

One round of dealings of all the factions. In my campain I run a round after each in-game day.

## Countdown clocks

Every obstacle for a faction has a number assigned that signifies how long the faction needs to work on it, until it overcomes it.
I organize the obstacles as grim potents in *World style fronts.

## Fronts
Fronts work almost the same as I am used to in Dungeon World. There are three notable differences.
* every grim potent has a countdown assigned
* fronts has oposition in adition to cast, where cast lists factions wanting the front to complete, while oposition wants to stop it
* grim potents of different fronts can influence each other, i.e. if two factions have "They stole the McGuffin" potent, that they strive towards, when one faction completes it, other has to change their plans.

In next paragraphs, I might use words obstacle, grim potent and front sort of interchangeably. I probably do this, because factions attempt to further their agenda by bringing a front to its completion. Because fronts consist of list of grim potents, there allways is a grim potent that requires their attention.

## Goal

Every faction has a primary motivation, that signifies which obstacles does it want to tackle first.

## Reach

Every faction has *reach* (0 - 3), marked by ◀ that signifies, how many obstacles it can tackle in one turn. Rule states, that each turn it can try to overcome a single obstacle that aligns with its goal and number of aditional obstacles equal to its reach rating. 

## Effect

Every faction has an effect rating 0 - 3, marked by ◆ on the sheet, that it can use to roll to overcome an obstacle.

*Roll with effect rating X*  proceeds like this:
* roll X d6 dice
* take the highest number
 * if there was more than one 6, advance countdown by 6, this is a critical success
 * if 6, advance countdown by 4, this is a regular success
 * if highest number was 4 or 5, advance countdown by 2
 * otherwise advance by 1
* if X is 0, roll 2d6 and take a lower result

Obstacle is overcome after its countdown is reduced to 0.

If it makes sense in a fiction, a faction might want to try to roll to set the countdown back. 
Some if some faction might try to tear down a river dam, other might want to repair it. 
Keep in mind two things. 
* Factions goal should always compel faction to count down some grim potents on some specific front.
* Fiction first. If the river dam was broken and the village has been flooded, there is probably no faction that could make it un-flooded.

After an obstacle has been overcome, check whether it implies or prevents fulfilment of other grim potents. 

## Faction Relations

Every faction has a relationship rating with every other (-3 - +3). 
Every time faction tries to overcome an obstacle/further its grim potent countdown, 
it can try to ask another faction for a helping die, increasing the effect by 1 for this roll.

1. YH, the relation between the faction rolling and helper
2. HO, the relation between helper and faction that would be opposed to the roll, if such faction exists
3. He, the effect rating of the helper.

You then calculate (YH - HO) what signifies, how much do they want to help you in this task.
1. If (YH - HO) < 1, then faction recieves no helping die.
2. If 0 < (YH - HO) < He, then faction recieves (YH - HO) helping die.
3. else faction recieves He helping die.

Every turn, each faction can help only as many times as many actions can it do itself (i.e. maximum is 4, minimum is 1) 

If the roll with help was a success (meaning, at least one 6), add the helper to the cast on the front. (or oposition, if you were rolling to set a front back)

##  When Faction wants to roll rolling to overcome an obstacle

1. Mark another ◁. You can mark at most one more ◁ as the faction has already marked ◀. If it doesn't have any free ◁, it can't attempt to overcome the obstacle.
2. it takes as many dice as it has *effect rating*
3. looks at its relationships to gather, whether there is someone do lend a helping die. If there is, mark another of their ✪. You can mark at most one more ✪ as the faction has already marked ◀, or the faction has no longer time to help.
4. rolls for effect rating with all the dice it was able to gather to resolve how far should it advance the countdown on the obstacle
5. advances the given countdown.
6. look at every faction that oposed overcomming of this obstacle and mark ☹ next to relationship.
7. if the clock was successfully completed, and somebody was helping, mark ☺ next to the relationship
8. if the clock was successfully completed mark ☺ next to every factions relationship that was hepled by overcomming this obsacle

## Before starting

1. Think about the stuff that is going to happen that you want to track
2. Think about the key npc players/factions
3. start filling out your fronts 
  * start with doom, stakes and grim potents
  * don't assign *cast* and *oposition* yet
  * don't assign countdown clocks to grim potents yet
4. Write down 4 most relevant factions, and fill their names in the faction graph
5. Think about the relation between fronts and factions
  * on each front 
    * list all the factions, that would actively work to further it under the *cast*
    * list all the factions, that would actively work to supress it under the *oposition*
6. Assign each faction the most important front they are in as a *goal*
7. Think about the ability/power/resources of each faction and assign the grey *effect* and *reach* ratings accordingly.
  * every faction on its turn can roll to further their agenda on the front that is their *goal*
  * for every mark in *reach* rating they can aid or interfere in another front
  * *effect* rating quantifies their ability to further their agenda
   * default is 1
   * 0 if you want to emphasize their ineptness
   * 2 if you want to emphasize ability
8. assign countdown clocks to grim potents
  * you might need the effect statistics to help you set some semblance of pacing
  * default is 4
9. draw a red line between grim potents that compete with each other, meaning where fulfilling one prevents fulfilment of the other
10. draw a green line between grim potents  where fulfilling one implies fulfilment of the other

## Regular turn

Every set ammount of time (in Dungeon world I either track one ingame day, or roll when players *make camp*)
for every faction do:

1. Roll on the obstacle that hinders to achieving the factions goal the most.
2. For every other unmarked ◁, faction can roll on obstacle it didn't roll this turn yet

After all factions are done, look at all ☹ and ☺ next to their relationship lines.
* If only ☺ is marked, mark +1 to relationship.
* If more ☹ are marked than ☺ mark -1 to relationship.

Look, if some front has no more obstacles listed as grim-potents. If so, 
  * faction that had fulfilled its goal by completion this front,
marks another ◆. 
  * all factions that helped, mark another ◀.

At the end, clear all of the ◁,✪,☺,☹ and your factions are ready to fight for another day (or week, not sure yet :).

# Rolling outside of the turn

There might be a time, when it makes no sense to wait for the end the day, because for example your PCs forced king to attack his rival. You can still roll on the faction sheet. Just remeber to mark all the ◁,✪,☺,☹, so that when the regular turn comes and it is time for the rest of the factions to catch up, you know who is too bussy already.

## Effect Statistics

I made myself a little table to help me gauge how long *in die rolls* a grim potent takes to advance. 

0. counts 1.3 down on average
1. counts 1.8 down on average
2. counts 2.4 down on average
3. counts 2.8 down on average
4. counts 3.2 down on average

Therefore when considering the difficulty of a countdown, consider how many rolls you'd probably need to resolve this:
1. segment, gets resolved for everybody, automatically
2. segments, it is very likely it gets resolved in single roll
4. segments, it is possible it gets resolved in a single roll
6. segments, you would need a critical success
8. and more, it is impossible to succeed in a single roll
