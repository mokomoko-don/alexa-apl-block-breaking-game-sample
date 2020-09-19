# Block Breaking Game Sample

The "Blockbuster Game Sample" is a sample of a block-breaking game that runs in APL 1.4.

# ScreenDemo

! [screendemo](https://raw.githubusercontent.com/mokomoko-don/alexa-apl-block-breaking-game-sample/master/images/block_breaking.png)

# Features

This code runs on alexa, which is implemented in the Amazon Echo Show series and others.

New in APL 1.4, we took advantage of new gesture support and handleTick to create a block-breaking game.

# Requirement

 * Actual device running Alexa
 * AlexaDeveloperConsole account
 * Knowledge of simple custom skill creation

# Installation

In addition to running it as a custom skill, you can also run it on the APL editor in the development console (in APL source code only).

## How to activate it as a skill during development

 * Create a HelloWorld skill in AlexaDeveloperConsole (AlexaHostedSkill).
 * Enter any skill name.
 * Press "Interfaces".
 * Enable "Alexa Presentation Language".
 * Press "Save Interface".
 * Go to "Interaction Model" -> "JSON Editor".
 * Copy and paste "/interactionModels/custom/ja-JP.json".
 * "Save Model" and "Build Model".
 * Go to code editor.
 * Copy and paste all files under "/lambda".
 * Replace line 524 of /lambda/APL/renderDocument_sample.json with the actual image URL (it will work without the background).
 * Save and deploy.
 * Go to the "Test" screen.
 * Change "Off" to "Development" in the pull-down menu.

## How to run on the APL editor

 * Create a HelloWorld skill in AlexaDeveloperConsole (AlexaHostedSkill).
 * Enter any skill name.
 * On the "Build" screen, go to the "Multimodal Responses".
 * Press "Visual" and "Create Visual Response".
 * Press "Upload Code".
 * Load "aplEditor/apl_template_export.json".
 * Press "Save Template" at the top right of the screen.

# Usage

## How to activate it as a skill during development

Launch from the actual device with "Alexa, open *****".
(Not verified in the PC simulator.)

## How to run on the APL editor

On the APL Editor screen, press the actual output button at the bottom of the output simulation.
(Try it in preview mode on a PC.)

## How to play

Touch and drag the pad to eliminate the block to avoid dropping the ball down.

Depending on the position of the ball that hits the pad, the reflection angle of the ball changes.

There is no direction to clear the game.

# Note
As of September 2020, the system has been confirmed to work. Please note that we do not guarantee the operation when it stops working due to specification changes in the future.
There seems to be a bug that prevents blocks from disappearing in rare cases. If you're confident, try to fix it!

# Author

* kyukkyu
* Twitter : https://twitter.com/Synoyan

# License

"Block Breaking Game Sample" is under [MIT license](https://en.wikipedia.org/wiki/MIT_License).
