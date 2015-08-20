# README #

### What is this repository for? ###

* SquareBattle is a game written in LabVIEW where you create your own squares to compete against other peoples squares in the arena.


### How do I get set up? ###

* [Clone this repository](https://confluence.atlassian.com/display/BITBUCKET/Bitbucket+101) somewhere on your computer, or alternatively, download the current version and unzip it somewhere on your computer.
* In the LabVIEW project you will find some folders containing example Squares (Carl, Robert and Shawn), a folder of utility vis including the arena vis, the class "Square.lvclass" and then finally SquareBattle Main.vi, which when run launches the arena.

### Running the game ###

Launch the project and run SquareBattle Main.vi. Select the Squares to compete and click Start Battle. The Squares will duke it out until there's only one left or the timer runs out.


### Creating your own square ###

* To create your own Square competitor it must inherit from Square.lvclass and it must reside in the "Squares" auto-populated folder. Also, it must override the methods "Player Info.vi" and "Run.vi". Player Info is called once when the arena is launched and allows you to name your Square competitor as well as specify a victory phrase which is displayed when you win.  The Run method is called every tick once the game starts. The tick time is currently user adjustable during the game. Your square can Wait, Move, Attack, or Replicate. Wait, Move and Attack each take one turn, Replicate takes 100 turns. To start out there are several example classes to pick from that can do battle. These are all within the Square folder. Shawn's Wanderer and Explorer classes are excellent opponents to go up against as you develop your own class.
* As soon as your class is created and "Player Info.vi" and "Run.vi" are overridden, your Square will show up in the list of players.  In order for them to show up in the executable, you will need to run the "Class Source Distribution" build specification.


### Who do I talk to? ###

* shawn@endigit.com, carl@endigit.com or robert@endigit.com