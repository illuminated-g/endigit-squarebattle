# README #

### What is this repository for? ###

* SquareBattle is a game written in LabVIEW where you create your own squares to compete against other peoples squares in the arena.


### How do I get set up? ###

* [Clone this repository](https://confluence.atlassian.com/display/BITBUCKET/Bitbucket+101) somewhere on your computer, or alternatively, download the current version and unzip it somewhere on your computer.
* In the LabVIEW project you will find some folders containing example Squares (Carl, Robert and Shawn), a folder of utility vis including the arena vis, the class "Square.lvclass" and then finally SquareBattle Main.vi, which when run launches the arena.

### Running the game ###

* Launch the project and run SquareBattle Main.vi. Select the Squares to compete and click Start Battle. The Squares will duke it out until there's only one left or the timer runs out.


### Creating your own square ###

* To create your own Square competitor it must inherit from Square.lvclass (after you open the project, right click on "My Computer"->New->Class to create a class, then change the inheritance by right clicking on the class, going to properties->inheritance->"Change Inheritance" and then select "Square.lvclass")  and it must reside in the "Squares" auto-populated folder. Also, it must override "Run.vi" (Right click on the class after it is set up to inherit from the Square.lvclass, choose new->"vi for override" and select "Run.vi"). 
* In order for your squares to show up in the list of competitors you also must override "Player Info.vi" which is called once when the arena is launched and allows you to name your Square competitor as well as specify a victory phrase to be displayed when you win.
* For examples of what the "Player Info.vi" and "Run.vi" should look like, look at any of the example squares in the "Squares" folder. If a class doesn't override the "Player Info.vi" you can still choose to launch that file when you Replicate (see below) but it won't show up in the list of initial players.
* The Run.vi method of each square on the board will be called once every tick once the game starts. After all of the "Run.vi" data has been collected, the arena will be updated. The tick time is currently user adjustable during the game.
* The Run.vi has as an input a 3x3 2d numeric array where the middle value represents your square and the rest represent the board immediately surrounding your square with 0 indicating an empty square -1 indicating an enemy and any positive numbers representing one of your own squares. Your job is to take that array, decide what to do, and then respond with an Action and a Direction to take that action in (as well as a Class if you are replicating). 
* The available actions are Wait, Move, Attack, or Replicate. Wait, Move and Attack each take one turn, Replicate takes 100 turns. When you Replicate you can pick the class of your new square. So, for example, you could have an initial square that just replicates, but when it replicates, the new squares are squares that move around and look for enemies.
* To start out there are several example classes to pick from that can do battle. These are all within the Square folder. Shawn's Wanderer and Explorer classes are excellent opponents to go up against as you develop your own class.
* As soon as your class is created and "Player Info.vi" and "Run.vi" are overridden, your Square will show up in the list of players when you run SquareBattle Main.vi directly.  In order for your squares to show up in the executable, you will need to run the "Class Source Distribution" build specification.


### Who do I talk to? ###


* shawn@endigit.com, carl@endigit.com or robert@endigit.com