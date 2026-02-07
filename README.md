# ULTRAPOL
ULTRAPOL is an unofficial subset of another Github project called "ULL" (short for "Ultrakill Language Library").
Given you have both BepInEx and ULL installed, the files presented in this repository will allow you to play Ultrakill with both polish text and font.

## Notes:
- I'll be occasionally making changes for the translation, this one isn't final.
- While we translated text to polish and provided a font with polish support, I didn't translate textures, nor voicelines. There are other polish teams that did the dubbing, but I don't know if they finished their work.
- Ultrakill uses a VCR OSD MONO font, which doesn't have polish characters, and the official ULL release also does not. You'll have to replace the **ullfont.resource** file with the one I provided.
- Few lines may be missing, I'll be comitting improvements from time to time

## How to install
1. Get access to the steam ULTRAKILL directory
	- Open Steam
	- Find **ULTRAKILL** in your **Library** page
	- Press the **Gearbox icon**
	- Press **Manage**
	- Press **Browse local files**
  
2. Install BepInEx (it's a mod framework, needed to run the ULL mod)
	- Download [**BepInEx_win_x64_5.4.23.4.zip**](https://github.com/BepInEx/BepInEx/releases/download/v5.4.23.4/BepInEx_win_x64_5.4.23.4.zip) (use this link if you need another version https://github.com/BepInEx/BepInEx/releases)
	- Paste all the contents directly to the <ins>**ULTRAKILL**</ins> folder

3. Install ULL (it's a translation mod, needed to load the polish text)
	- Download [**UltrakULL-1.3.1-Beta.zip**](https://github.com/ClearwaterUK/UltrakULL/releases/download/v1.3.1-beta/UltrakULL-1.3.1-Beta.zip) (use this link if you need another version https://github.com/ClearwaterUK/UltrakULL/releases)
	- From the <ins>**downloaded ULL zip folder**</ins>, take <ins>**config**</ins> and <ins>**plugins**</ins> and place them in <ins>**ULTRAKILL/BepInEx**</ins> (even if the BepInEx folder already has config and plugins)
	- Run the game to see if you have properly installed everything (You should see a **Language** tab in your options menu)
	
5. Add polish text
	- Go to: <ins>**ULTRAKILL/BepInEx/config/ultrakull**</ins>
	- There, place the **pl-PL.json** file

6. Add polish font
	- Go to: <ins>**ULTRAKILL/BepInEx/plugins/UltrakULL**</ins>
	- There, replace the **ullfont.resource** with the one I provided

7. Enable the polish language
	- Open the game
	- Go to **Options**
	- Go to **Languages**
	- Select the Polish language
	- Now you'll be able to play Ultrakill with polish text and font. Enjoy :]

8. (Bonus, optional) Hide the BepInEx console
  - Go to: <ins>**ULTRAKILL/BepInEx/config**</ins>
  - Open the **BepInEx.cfg** file in a text editing software.
  - Find the **[Logging.Console]** section
  - There, you will see a variable **Enabled**. Change its value from *true* to *false*
  - Now, the console won't open everytime you open the game