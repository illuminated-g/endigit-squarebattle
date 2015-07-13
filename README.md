# README #

### What is this repository for? ###

* SquareBattle is a game written in LabVIEW where you create your own squares to compete against other peoples squares in the arena.

### How do I get set up? ###

* [Clone this repository](https://confluence.atlassian.com/display/BITBUCKET/Bitbucket+101) somewhere on your computer, or alternatively, download the current version and unzip it somewhere on your computer.
* In the LabVIEW project you will find some folders containing example Squares (Carl, Robert and Shawn), a folder of utility vis including the arena vis, the class "Square.lvclass" and then finally Main.vi, which when run launches the arena. 
* To create your own Square competitor it must inherit from Square.lvclass and it must reside somewhere in the folder structure where the project resides. Also, it must override the methods "Write Player Info.vi" and "Run.vi". Write player info is called once when the arena is launched and allows you to name your Square competitor as well as specify a victory phrase which is displayed when you win.

### Running the game ###
Launch the project and run Main.vi. Click on Start Battle. Browse to your .lvclass that controls your squares. This class must be a descendant of the Runner.lvclass and should have a Run method and should reside in the project folder structure. The Run method is called every tick once the game starts. The tick time is currently user adjustable during the game. Your square can Wait, Move, Attack, or Replicate. Wait, Move and Attack each take one turn currently. Replicate takes 100 turns. To start out there are several example classes to pick from that can do battle. These are all within the Runner folder. Shawns Wanderer and Explorer classes are excellent opponents to go up against as you develop your own class. 



### Who do I talk to? ###

* shawn@endigit.com, carl@endigit.com or robert@endigit.com