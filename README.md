This Github contains the Port of PMD:Tranquility for Foundry VTT and a Foundry Module for a few necesary assets.

Importing the templates:
- Instal Custom system builder on your Foundry (https://foundryvtt.com/packages/custom-system-builder)
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

I recommend copying the example actor (Zeraora) and making new characters from it (active effects are weird to add to a brand new actor for some reason)
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/1e7a111e-5295-4bf4-8a42-72fb1a0fc32c" />


Quasi necesary external module:
- [Carolingian UI](https://github.com/crlngn/crlngn-ui) (Port was made with this this module in mind, the character sheet will look off without it. Additional CSS needs to be added through it)

Recommended modules:
- https://gitlab.com/mxzf/status-halo/-/releases
- https://gitlab.com/riccisi/foundryvtt-dice-so-nice
