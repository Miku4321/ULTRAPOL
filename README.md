[![en](https://img.shields.io/badge/lang-en-blue.svg)](https://github.com/Miku4321/ULTRAPOL/blob/main/README.md)
[![pl](https://img.shields.io/badge/lang-pl-red.svg)](https://github.com/Miku4321/ULTRAPOL/blob/main/README.pl.md)

# ULTRAPOL
ULTRAPOL is an unofficial subset of another Ultrakill mod called "ULL" (short for "Ultrakill Language Library").
<br/>Given you have both BepInEx and ULL installed, the files presented in this repository will allow you to play Ultrakill with both polish text and font.

## What content does this mod translate
- [x] Text (e.g. subtitles, interface, books, enemy names, weapon descriptions)
- [x] Font
- [ ] Textures (e.g. text on walls)
- [ ] Voicelines (i.e dubbing)

## Notes
- I'll be occasionally making changes for the translation, this one isn't final, especially given some lines are empty. I also *might* translate some of the textures
- While we translated text to polish and modified the font to have polish support, I didn't translate the textures, nor voicelines. There are other polish teams that did the dubbing, but I don't know if they finished their work
- Ultrakill uses a VCR OSD MONO font, which doesn't have polish characters, and the official ULL release also does not. This results with the game using an ugly fallback font. To prevent this, you'll have to replace the **ullfont.resource** file with the one I provided (section "How to install" will provide the instructions)
- As of the time of writing this (7th February 2026), the newest version of ULL (1.3.1 beta) is intended for the "ULTRA_REVAMP" update of Ultrakill (patch 16d). The future Fraud update may break the mod.

## How to install
1. Get access to the ULTRAKILL directory
	- Open Steam
	- Find **ULTRAKILL** in your **Library** page
	- Press the **Gearbox icon**
	- Press **Manage**
	- Press **Browse local files**
  
2. Install BepInEx (it's a mod framework, needed to run the ULL mod)
	- Download [**BepInEx_win_x64_5.4.23.4.zip**](https://github.com/BepInEx/BepInEx/releases/download/v5.4.23.4/BepInEx_win_x64_5.4.23.4.zip) from [BepInEx releases](https://github.com/BepInEx/BepInEx/releases)
	- Paste all the contents directly to the <ins>**ULTRAKILL**</ins> folder

3. Install ULL (it's a translation mod, needed to load the polish text in-game)
	- Download [**UltrakULL-1.3.1-Beta.zip**](https://github.com/ClearwaterUK/UltrakULL/releases/download/v1.3.1-beta/UltrakULL-1.3.1-Beta.zip) from  [ULL releases](https://github.com/ClearwaterUK/UltrakULL/releases)
	- From the <ins>**downloaded zip folder**</ins>, take <ins>**config**</ins> and <ins>**plugins**</ins> and place them in <ins>**ULTRAKILL/BepInEx**</ins> (even if the BepInEx folder already has config and plugins)
	- Run the game to see if you have properly installed everything (you should see a **Language** tab in your options menu)
	
4. Add polish text
	- Go to: <ins>**ULTRAKILL/BepInEx/config/ultrakull**</ins>
	- There, place the **pl-PL.json** file

5. Add polish font
	- Go to: <ins>**ULTRAKILL/BepInEx/plugins/UltrakULL**</ins>
	- There, replace the **ullfont.resource** with the one I provided

6. Enable the polish language
	- Open the game
	- Go to **Options**
	- Go to **Languages**
	- Select **Polski (Polish)**
	- Now you'll be able to play Ultrakill with polish text and font. Enjoy :]

7. (Bonus, optional step) Hide the BepInEx console
	- Open <ins>**ULTRAKILL/BepInEx/config/BepInEx.cfg**</ins> in a text editing software
	- Find the **[Logging.Console]** section
	- There, you will see a variable **Enabled**. Change its value from *true* to *false*
	- Now, the console won't open everytime you open the game