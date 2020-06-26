# zootr-router
Very WIP automated routing recommendations for Ocarina of Time Randomizer seeds

Main function is parseLogicFT. This converts logic files in the specified path to OpenPSA format fault trees. These can be solved for the minimal logical combinations using SCRAM (https://github.com/rakhimov/scram). Cutsets can then be converted into bitarrays or whatever format is necessary for the router engine.

OoTR logic files use a number of shorthand functions expanded via AST, presumably to make the logic more human-readable. testLogic is used to screen every phrase in the logic file for any that are not yet handled.