# README #

### What is this repository for? ###

* SquareBattle is a game written in LabVIEW where you create your own squares to compete against other peoples squares in the arena.

### How do I get set up? ###

* Clone this repository somewhere on your computer. Launch the project and run Main.vi. Click on Start Battle. Browse to your .lvclass that controls your squares. This class must be a descendant of the Runner.lvclass and should have a Run method. The Run method is called every tick once the game starts. The tick time is currently user adjustable during the game. Your square can Wait, Move, Attack, or Replicate. Wait, Move and Attack each take one turn currently. Replicate takes 100 turns. To start out there are several example classes to pick from that can do battle. These are all within the Runner folder. Shawns Wanderer and Explorer classes are excellent opponents to go up against as you develop your own class. 

*Strategies:


### Who do I talk to? ###

* shawn@endigit.com, carl@endigit.com or robert@endigit.com