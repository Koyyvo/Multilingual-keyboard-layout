# Multilingual-keyboard-layout

----------
## Purpose
To make multilanguage keyboard configuration(s). 

Take note that, as the layouts are custom, to use them you'll probably have to have a keyboard custom-made (or at least some of the keys).

Layouts are based on the ISO-105 keys standard


----------
## Current situation

Most keyboard configurations don't allow users to write in a lot of languages, even if it would be possible. Some examples:

"English (US)" keyboard config includes the tilde (~), but not as a deadkey, so English (US) users cannot make the accentuated characters for the following languages: Spanish, Portuguese, Estonian (ñ, ã, õ). Spanish keyboards often have ñ as a dedicated key 

French keyboards than includes the cedilla (¸) as a deadkey only have ç configured. Some French keyboards don't even have the cedilla deadkey: they have ç as a dedicated key. Languages using the cedilla in more than the ç form: Portuguese, Latvian, Lithuanian, Polish, Romanian.


----------
## Keyboard layout guide

A layout is comprised of 5 states. Default is what you type normally; the other 4 requires the user to maintain the key(s) to type the character associated.
- Default
- Shift
- Alt+Ctrl (or Alt Gr)
- Ctrl
- Alt+Ctrl+Shift


----------
## Definitions

Deadkey: name used to refer to the key used to add a diatric on a character
https://en.wikipedia.org/wiki/Dead_key

Accentuated letter: it is of note that throughout this project, every letter using a diatric is considered to be "accentuated". This is important, considering most languages consider "diatric'd" letters to be whole letters; a lot even have dedicated keys on specific language keyboard configurations (again, ñ in some Spanish, ç in some French configurations)


----------
## Sitemap

Example for the first layout (FrCa-multi.klc):

 - [layouts] -
	 - [FrCa-multi] -
		 - [Diatrics (Windows).ods]: included diatrics/special characters, with Windows-specific codes for configuration (linux ones might be added in this file) 
		 - [Language compatibility list.ods]: languages users should be able to write in with the keyboard configuration. (Includes languages users might be able to write in with some additions)
		 - Windows - 
			 - [FrCa-multi.klc]: layout, based on the Windows "French (Canada)", that
	   includes most of the diatrics in the [Diatrics (Windows).ods] as deadkeys.
			 - [Keyboard Layout Creator verification file]: gives warning regardings
	   compatibility issues.
		 - Linux -
			- [layout] (in the *To Do* list)


----------
## To do
#### Primary work:
- As seen in Windows - ods some languages require diactrics not included in the present layout. Add those.
- Add an easy way to visualize the layouts.
- Add linux configurations to match Windows ones.
- Add latin languages possibilities (and add to the .ods file possibilities already there but left out of the file).
- Add multi-alphabet option (Greek, cyrillic). The goal here is to have, say, the 26 basic latin letters (from English, as this is the basic of the project for now) sharing their design with the 24 greek letters. Of course, you'd have to switch configuration, but the "keyboard design" would be the same. See image left to right: latin (primary) Z with greek ζ; greek ζ (primary) with latin Z.
- Add greek and cyrillic as primary options.
- Find a better way to include special characters, if possible.

<img width="150" alt="Key example with the Z and ζ letters. Latin to greek. Greek to latin." src="https://raw.githubusercontent.com/Koyyvo/Multilingual-keyboard-layout/master/assets/img/multilanguage-key-example.jpg">

### Secondary work:

 - Add 104-keys configurations.  
 - Make alternative keyboards layout to the QWERTY used. (This refer only to the 26 letters layout. An
   alternative would be AZERTY, for example). 
 -  Make languages specific layout. This means that, even though the goal is to make
   multilanguages layouts, most people use one language more. As an
   example, to write in French, people may prefer to have [default] é [shift] É [Alt Gr] ´, instead of [default+shift] ´.




----------
## Ressources

**Atom**, to open the Windows .klc files (UTF-16 encoding required to read the files) : https://atom.io/

Windows **Keyboard Layout Creator** : 
https://www.microsoft.com/en-us/download/details.aspx?id=22339

WASD offers a virgin keyboard layout in vector formats. You can also print it to draft: 
https://support.wasdkeyboards.com/hc/en-us/articles/115007847008-Download-Template-Files 

For Linux, explore the following options:
https://askubuntu.com/questions/92751/create-my-own-keyboard-input-layout


----------
## Disclamer

Most of the information included in the .ods files comes from Wikipedia. Some may be wrong or may require precision. Native speakers are welcome to add those as required.
