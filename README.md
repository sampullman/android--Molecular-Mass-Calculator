# Molecular Mass Calculator
### by Sam Pullman

This is an Android app that computes the mass of any molecular formula. Other features include:
* Displays mass percentages of each element in the input formula.
* Attempts to grab the name of the formula with an HTTP query to a government database.
* Portrait and landscape modes.
* Prompts user to resolve ambiguous formulas with a list of all the possibilities.

## Instructions for getting this project up and running from the command line.

If you are an Eclipse/IntelliJ/NetBeans user you should replace any shell commands with an action appropriate to your IDE.
The 'update command' I will be referring to is simply:
android update project -p .

1. Clone this repository to a directory of your choice. This directory will be referred to as PROJ_HOME.

2. cd into PROJ_HOME/MolecularMassCalcLib/ (up one level) and run the update command.

3. cd into PROJ_HOME/MolecularMassCalcPaid/ and run the update command. If you wish to build the free version, run the command in MolecularMassCalcFree.

4. The project is now ready to be built. There is a script included in the Paid/Free directories called "run" that cleans, debugs, and installs the app on whatever device you have connected. You can use the standard ant commands (clean, debug, etc.), although to release you would have to use your own keystore and refer to it in the ant.properties file in both the Lib and Paid/Free directories.

5. Make changes in the MolecularMassCalcLib project, and they will be reflected in both the Paid and Free projects. All you need to do is build the Paid/Free project and install it. Note that the Lib project cannot be installed as a standalone app.

6. Let me know if you have any issues or questions.