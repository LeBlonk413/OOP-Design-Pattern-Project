# Design Patterns - OOP Project

- Pokemon Minigame -

UPDATE PATTERN

The abstract class Update will call all the other update functions, in this
case the functions (added with the functions from BattleEditor) are updating
HP, status, and ability cooldown from the BattleUpdateCD and
BattleUpdateHpStatus classes.

OBSERVER PATTERN

The class Battle represents the observer pattern, while the "subscribers" are
part of the class Pokemon. Every time a pokemon battle ends, each pokemon
gets an update so they can reset their stats for the next fight.

FACTORY PATTERN

This pattern allows the creation of Neutrel Pokemon at ease, using the 2
hardcoded classes that extend Pokemon, Neutrel1 and Neutrel2.

SINGLETON

The Neutrel class is in itself a Singleton, which makes sure that we won't
create more than one instance of it when creating a Neutrel Pokemon.

-------------------------

There are 4 adventures, each with 3 battles in order. For the first battle both
of the trainers will go against a Neutrel1, for the second they will go against
a Neutrel2, and the last fight is a PvP fight between the 2 trainers.

For each adventure, the trainers will use one pokemon only, in order: 1st, 2nd,
3rd, and their best total stats pokemon.

-------------------------

The Pokemon details are stored in a json file, from which the program will
create a map with all their information, stored with the key=pokemon name.

Same for items.
