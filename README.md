# README #
Quick notes regarding Rev 2:

1. Added Stats!
2. The map that is the input to run.vi is now a 1D array that can be indexed by the direction enum.
3. The 1D array map has -1 for an empty space and then the team number of the square if it isn't ampty. For example, an array of [-1,-1,0,10,-1,-1,-1,-1,-1] would indicate empty squares all around you except someone from team 0 to your NE and someone from team 10 to your E.
4. Your own team # is an additional input to Run.vi
5. There is a new vi (Eliminated.vi) you can override that is only called once, when your team is obliterated and gives you the name of the team that did it.
6. Speaking of obliteration, Player Info now includes a phrase to be shown when you are obliterated.
7. Players position on the map is given to them via a "row" and "column" input where 0,0 is in the bottom left corner and increases towards the top right corner.
8. More efficient and spiffy
9. Updated the Documentation

For detailed instructions, please download and review the following PDF: 
[SquareBattle Instructions](Documents/SquareBattle_Instructions.pdf).

For the SquareBattle projct saved back to LabVIEW 2013, see the [LV2013 Repository](https://bitbucket.org/endigit/squarebattle-lv2013).
### What is this repository for? ###

* SquareBattle is a game written in LabVIEW where you create your own squares to compete against other peoples squares in the arena.


### How do I get set up? ###

* [Clone this repository](https://confluence.atlassian.com/display/BITBUCKET/Bitbucket+101) somewhere on your computer, or alternatively, download the current version and unzip it somewhere on your computer.
* In the LabVIEW project you will find a folder named "Documentation". In that folder is the SquareBattle Instructions PDF I mention above. Grab some popcorn and settle down for some good reading. It will be worth it! No, really, you should read it.

### Running the game ###

* Launch the project and run SquareBattle Main.vi. Select the Squares to compete and click Start Battle. The Squares will duke it out until there's only one left or the timer runs out.

### Who do I talk to? ###


* shawn@endigit.com, carl@endigit.com or robert@endigit.com