## The relationship-frons worksheet

This worksheet is supposed to help you, when multiple npcs (or groups of npcs) are trying to advance
different competing fronts, while interacting with each other.

You can consider this repo [CC BY-SA-NC](https://creativecommons.org/licenses/by-sa-nc/2.0/) licensed, so you can hit that fork button,
and edit to your hearts content, just beware, that I have just begun experimenting, and have no idea what will adhering to these rules
do to pacing your campaign :) Well, that is unless John Harper tries to stop this from circulation, because I take one of his core mechanics from his not released game.

These rules take from John Harpers [Blades in the Dark](https://www.kickstarter.com/projects/2080350433/blades-in-the-dark) 
and Sage Kobolds [Dungeon World](www.dungeon-world.com/) and Vince Bakers [Apocalypse World](http://apocalypse-world.com/) fronts.

What kicked me into hacking was this specific [episode of Hack Attack](https://www.youtube.com/watch?v=ual1y1O7x1A) where Adam Koebel 
and Steven Lumpkin discuss porting Stars Without Number faction turn to support the  [West Marches](https://www.reddit.com/r/itmejp/comments/2idf33/west_marches_resources/) style play better in DnD 5 on [RollPlay](http://itmejp.com/rollplay/) by ItmeJP

My intentions are:
* Have fronts account for differing difficulty of different grim potents
* Model oposintion among fronts cast
* Model fronts casts differing in power
* Have the rules simple enough, so that you can advance the front in 1 to 3 minutes.

First, lets re-iterate how fronts in Dungeon Wolrd work (because that is the system, that I currently run).

Front is a tool to help the GM to organize oranize their thoughts
on what oposes the players. Each front should consist of:

1. a `name` i.e.: "Waking of the Elder God"
2. an `impending doom` that comes to pass if players dont stop the progressing front i.e.: "Elder God wakes up and the world goes MAD!"
3. list of `dangers` that this front manifests i.e.:
 * A curse of madness that haunts the catacombs (impulse *to ensnare*)
 * Dark Cultists (impulse *to follow their MAD doctrine*)
 * Eldritch Abomination (impulse *to wreak havoc without care*)
4. a `cast`, naming specific key NPCs and giving a face to dangers
 * High Preast
5. list of `grim potents` that show how the front progreses towards the manifestation of its doom, i.e.:
 * Cultists gather in taverns backroom for a meeting
 * Cultists break in and steal the tome Al-Mukhtaá¹£ar fÄ« Al-Jabr in the mansion of mad cartographer Al Chawarizmi
 * Cultists open the door to catacombs with the key of their order
 * Cultists find the tomb an use the tome to awake the Eldritch

There might be multiple fronts. For example if there was a second front about 
derelict ship with treasure, it might look like this:

* `name`: The treasure hunt
* `impending doom`: wreck sunks and nobody gets the treasure
* `dangers`: Undead pirates (impulse `protect the gold`)
* `cast`: Undead pirates
* `grim potents`:
 * you can see the rising tide
 * water seeps into cargo-hold
 * cargo-hold is flooded
 * deck has water up to ankles
 * ship sinks into the abyss

You as the GM advance fronts that are applicable when:
* Players fail a roll
 * i.e.: Player is in cargo hold and fights a skeleton. Instead skeleton dealing damage, you could let water enter the cargo hold and flood it.
* Players look at you with question "What happens next?"
 * i.e.: GM: "You all gathered around the tavern table" P: "Do I see anything strange?" GM: "You might sevral hooded figures enter and head for the back room."
* The completion of front is implied by fiction, player action or inaction, i.e.:
 * Players loot the entire Al Chawarizmi mansion. You could then ask them, whether they want to destroy the tome or sell it to cultists.
    * If they sell it you can advance Cultist front  front to the catacomb door.
    * If they destroy it, the front progression has stopped
 * If players steal the tome from Al Chawarizmi mansion, and then they decide, that they want to loot the wrecked ship, when they enter the wreck, water should already seep into the cargo-hold 

This tool works best in my opinion if:
1. The grim potents are *binary*, meaning they either happened, or didn't.
2. Different fronts don't interfere with each other

Dungeon World solves the first problem by nesting fronts into each other. In my current cultist example, when players enter the Al Chawarizmi mansion,
I would think about the mansion as if it were dungeon with traps and different enemies advancing, and write a smaller-scale dungeon front for it. 

If the fronts interact with each other, it is on you as a GM to advance them as you see fit, what might pose a challenge for the fiction.

Consider a front:

* `name`: The maddening heist
* `impending doom`: mad thieves now roam the catacombs 
* `dangers`: Thieves (impulse `to go for s bigger heist`)
* `cast`: Thieves guild
* `grim potents`:
 * Thieves raid the Al Chawarizmi mansion and steal all the valuables including the tome
 * Thieves investigated the tome and learned about riches in the catacombs and the cultist key to open them
 * Thieves secretively steal the key from Cultist hideout
 * Thieves open the catacomb door and enter
 * The curse ensnares them and now mad thieves roam the catacombs

Now if players interact with the mansion at the begining of the campain, there is fun to be had with thieves, cultists and your players all trying 
to loot the mansion. But if players decide to spend the first day on the ship, how should I decide who gets to the tome first? Right now, as my example fronts stand,
it would seem that cultist plans got thwarted mostly because of their love for shadowy meetings, because when I advance the fronts, by the time cultists are done discussing,
the mansion is already raided. And because I like to be surprised in my game even when I GM, and conficting fronts like this got me thinking aong these lines:

* maybe the cultist meeting is just a standup-session and they are done in 5 minutes
* maybe even thieves like to plan their heists for hours 
* why wouldn't thieves sell the tome to cultists, do they hate them more than they love money?

That's why I propose to mechanize fronts by adding clock mechanism from Blades in the Dark.

After some deliberation I have gravitated towards these rules for my Faction-fronts:

A faction-front adventure consists of:
* 4 factions at most (because you want to have a relationship-graph between them that is complete and planar), where  each faction has
 * a name
 * a goal
 * reach rating 0 ... 3
 * effect rating 0 ... 3
 * a leverage marker for every other faction
* a line between every two factions that demonstrates their liking for each other on a scale -3 .. 3
* 4 fronts, where each front has:
 * Doom and Stakes as usual
 * Cast split to Cast and Oposition
 * list of grim potents with asociated countdown clocks
* lines that pair the grim potents that influence each other

# Name

It is good for a faction to have a name. Keep it short, because it needs to fit into Cast and Oposition fields.

# Goal

Is the name of front faction is most interested in resolving (or stopping)
# Effect Rating

The core mechanic is taken from Blades in the Dark, meaning that a faction will roll with their effect rating to advance the countdown on a grim potent.

*Roll with effrct rating X*  proceeds like this:
* roll X d6 dice
* take the highest number
 * if there waa more than one 6, advance countdown by 6
 * if 6, advance countdown by 4
 * if highest number was 4 or 5, advance countdown by 2
 * otherwise advance by 1
* if X is 0, roll 2d6 and take a lower result

I made myself a little table to help me gauge how long *in die rolls* a grim potent takes to advance. 

0. counts 1.3 down on average per roll
1. counts 1.8 down on average per roll
2. counts 2.4 down on average per roll
3. counts 2.8 down on average per roll
4. counts 3.2 down on average per roll

This is especially useful when it makes sense, that the grim potent is contested over two factions.
This is why the front Cast and Oposition, where Cast can roll on effect to move the count down, while Oposition
can roll to restore the count back up.

Lets consider a micro front:

* `name`: Legions arive
* `cast`: Imperial Legion (Effect rating 3)
* `oposition`: Rebelling Fishermen (Effect rating 1)
* `grim potents`:
 * Imperials curb the rebellion (Counts douwn from 4)

You can see, that if Legions don't curb the rebellion in one fell swoop in its first roll,
it might ocupy them for several turns while they go back and forth with the Fisher Men. 

## Effect rating from fiction

I am not yet sure, how different effect ratings will interact (that is why I made the table above), so if you want to estimate pacing,
or kow how long a part of campaign should take, assign effect ratings after you created your fronts with countdown clocks.

But in my mind:

0. effect, somebody unlikely to succeed in affecting the world, kings little daughter, alchemist never leaving his aboratory. You track them, because you need to track their relationships and to see if they advance their might.
1. effect, the everyman
2. effect, above average
3. effect, the veteran 

## Effetct rating discussion

Right now, I don't simulate different types of effects, because I want to keep things simple. I am not yet sure, how the relationship bonuses (when in fiction a faction asks other for help) will affect the outcomes.

## Advancing Effect rating

Every time a front relevant to the factions goal gets resolved, tick off another mark in effect rating.

# Reach rating

This rating allows the faction to mingle in fronts that don't concern their goal. Every time, faction has a chance (in fiction) to advance front torwards their goal, they can roll, and if they are the cast or oposition in any other front, they can roll on as many, as is is their Reach rating. This means, that at least, the faction works on a single front, at most, they can work on all four. 

# Relationship rating

I added relationship rating to be able to simulate how likely are the factions to help each other.

They are tied to two mechanics. Descriptions will use *you* as a faction in question on its turn and *they* as *your* neighbours on
the relationship graph.

## When rolling you can ask another faction for help

This will increase your effect rating for this roll. And fortunately doesn't require graph theory to operate, but there is math :-)

So in case, that *you* need a *help* to advance a front against some *oposition*, to know, how much will the *helpee* aid you,
you will need to note:

1. YH, the relation between *you* and *helper*
2. HO, the relation between *helper* and *oposition*
3. He, the *helpers* effect rating. 

You then calculate (YH - HO) what signifies, how much do they want to help you in this task. If (YH - HO) > 0, then *you* will recieve *help*. *You* will then recieve (YH - HO) aditional dice for your roll, but this number is capped of by the helpers effect rating He.

This means, that even if *you* have a +3 rating with some peasant faction that has only 1 effect rating, thay can still give *you* only one helping die. 

## Relationships from fiction

I think about the relations in terms of how much would factions hinder/help each other in their spare time.

* +++ helping each other is highest priority
* ++  they help each other if they have time/resources
* +   they don't really help each other unless asked
* 0   they don't care about each other
* -   they don't want really hinder each other
* --  they will hinder each other if they have spare resources
* --- they are allways at each other's throats

This then serves as a hint when ending a turn of a faction with unspent reach, that points towards what would they do.

## Advancing Relationship rating

Every time you attempt to hinder someone directly mark aditional ☹ (if there still is empty one) next to the relationship. Every time you succeed in hindering someone directly make sure both of ☹☹ are marked next to the relationship. Every time you *succed* in advancing someone elses front in a way they would aprove of, mark a ☺.

At the end of a faction turn, look at every  line and ☺ ☹ ☹ pictograms besides it. If only ☺ is marked, mark +1 to relationship.
If more ☹ are marked than ☺ mark -1 to relationship.

# Fronts

You can mostly specify all your fronts as you are used to. 
You know who tries to achieve what and you specify the probable succesion of events by the list of grim potents.
Here I will go in more detail about the three main changes:

## Each grim potent has a countdown clock with several segments

Because you will roll an effect roll for a faction, when it tries to advance (or supress a front),
you need a way to track how successfull was the roll. 

When considering the difficulty consider how many rolls you'd probably need to resolve this:

1. segment, gets resolved for everybody, automatically
2. segments, it is very likely it gets resolved in single roll
4. segments, it is possible it gets resolved in a single roll
6. segments, you would need a critical success
8. and more, it is impossible to succeed in a single roll

Consider the time the front should take to complete unoposed, and how often do you want to roll. 
I usually think in days (we play Dungeon World, so I tie this mechanic to the "make camp" that mostly takes once pre in game day)

## Cast splits to cast and oposition

Because I have several factions, and want them work against each other, sometimes some NPC would work against the fullfilment of the front. 

## Fronts interact

They interact on the grim potent level, because often, one grim potent fictionally implies fulfilment of different grim potent, or its prevention. I.e. if thieves steal the tome from the mansion, cultist can't steal it from the mansion anymore :-)
