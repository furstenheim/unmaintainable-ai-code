* Create a simple website with hello world

* Create a javascript code that on load generates a board of 20 width and 10 height    

* This is a game, we start at phase 1 when we place the ships. We should have one ship of size 5x1, 1 ship of size
4x1, 2 ship of size 3x1. 1 ship of size 2x1. They appear on the left of the board. Each has a small icon to rotat
e, then they can be dragged to the board. They can only be placed on the left half of the board. There is a butto
n at the button that says Ready. The button is deactivated with a subtext saying "First place all boats". Once al
l boats are placed the button goes to green and it is activated


* I should be able to take back an already placed ship. Either by a button on the menu of the fleet, or by dragging
 out an already placed ship


* It should not be possible to place two ship together, there must always be space between them


* When dragging the ships it drags the whole menu, it should only show the pixels of the ship

* When the ship is placed, the menu on the left stays active, it should show dimmer to be clearer that it is already placed


* Remove the green check when placed. Remove button should be red, not gray, only the button, ships colour is correct


* When all ship are placed and green button is ready, when the green button is ready, the AI will secretly place si
milar ship on the right half of the board. Ship cannot overlap, nor be adjacent, not even diagonally. This ship a
re not displayed.

* Add a debug button so that I can see the position of the AI ships


* Let's start the game. Once the ready button is pressed, instead of an alert we will go to play mode. Per turns, t
he human and AI will choose a position where they think there is a ship. If a ship is hit, we show red, if water
is hit we show blue. Change the colour of player ships so they are green

* When I click on the AI territory, my hits do not show. Also remove the debug button

