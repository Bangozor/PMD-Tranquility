This Github contains the Port of PMD:Tranquility for Foundry VTT and a Foundry Module for a few necesary assets.

Importing the templates:
- Install Custom system builder (CSB) on your Foundry (https://foundryvtt.com/packages/custom-system-builder)
- Create a World
- Once in the world, in foundry's game setting, locate the "import templates JSON" and upload the JSON file

<img width="301" height="1005" alt="image" src="https://github.com/user-attachments/assets/98ae4573-0721-42cb-864b-d36ccb6e90a7" />


CSB Setup:
CSB only allows the import of templates, which means that you will have to manually change the initiative formula in the game settings like the picture bellow
<img width="779" height="679" alt="image" src="https://github.com/user-attachments/assets/9af273c3-ae07-4fd4-9cf6-df469350de50" />


For the CSS file:
Copy the contents of the file into Carolingian UI's settings (Interface settings -> Theme & Styles -> Custom CSS text box)
<img width="1597" height="886" alt="image" src="https://github.com/user-attachments/assets/b96c32ed-230d-4175-b1e9-833fcb7dbf15" />


For the Module (PMD-tranquility-assets):
Unzip the file into your foundry installation module folder (Main foundry file/data/modules)

Within the module you will find: Items such as a base for attacks and status move (and all the Types, present in each move in the form of a table to calculate type weaknesses), an example actor, and all the statuses present in Tranquility
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/1e7a111e-5295-4bf4-8a42-72fb1a0fc32c" />

**To add status effect to a character, you need to drag and drop each status effect from the compendium directly on that actor's token, not on the character sheet. Make sure that "Link actor Data" is turned on in "prototype token" before doing anything to a character, without this setting, changes made to a token will not be transferred to the main character sheet found in the "actor" section of the foundry UI, and once the token is deleted, all changes will be lost**
<img width="1069" height="979" alt="image" src="https://github.com/user-attachments/assets/c785a051-fd3f-41a1-ba21-c5a64f461433" />
<img width="561" height="540" alt="image" src="https://github.com/user-attachments/assets/3dfda981-39c4-4b85-ae95-ec81ac730384" />

Regarding The Type Table in moves:
After some testing, I found out that the type table section of moves becomes empty when exported to/from the module, or when moving from a character to the Item section of the foundry UI, but NOT when moving from the item section to a character. 
Due to this, you will have to manually fill one PC move's and one NPC move's type table manually (I recommend using the two "Move Base" found in the module for this), then drag that filled out move to a character, which will copy it, and modify it in the character sheet, there is no need to do this for status moves as they do not use the type table. This is quite convoluted but doesn't seem to have a way to be fix on my side since this looks like a foundry issue (I'll keep looking for a way around this).

Quasi necesary external module:
- [Carolingian UI](https://github.com/crlngn/crlngn-ui) (Port was made with this this module in mind, the character sheet will look off without it. Additional CSS needs to be added through it)

Recommended modules:
- https://gitlab.com/mxzf/status-halo/-/releases
- https://gitlab.com/riccisi/foundryvtt-dice-so-nice
