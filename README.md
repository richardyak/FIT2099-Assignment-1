# FIT2099-Assignment-1
Starting code for FIT2099 Assignment 1, 2017, at Monash University.  

Force

Design Rationale

We've decided to create a new Force class on it's own as Force does not exactly fall under entity or any other category. Each actor
class member would have a force object, wherein there will be a force value of an integer, with this integer stored within the class.
This integer will be used within force's class to check if lightsabres, mind controls and other force related abilities will be able to
be used. This force value will either be randomly generated or predetermined, depending on the different actors (for example, droids
would have 0 force on creation). This means that we would have to create the force object during the creation of the actor object. 

In detail, for example, to find if an actor can wield a Lightsabre, when the player chooses to pick the wield lightsabre option in the
action menu, it would call the an actors getForce function and checks if it fulfills a criteria of being able to wield a lightsabre (for
example, maybe a minimum of 50 force is required to wield the lightsabre) and then return a string of whether or not the actor
is able to wield it. If it is successful, the light sabre will be added into the backpack, otherwise, the lightsabre will be left on the
ground.

As for the force user's mind control, there would be another option on the action menu to choose this option, only applicable when the 
player object is on the same panel another actor object. This mind control is only usable on droids, where they have effectively 0 force.
