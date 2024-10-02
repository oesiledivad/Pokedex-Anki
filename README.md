<h1 align="center">Pokedex Anki</h1>
This deck will help you to memorize all 1025 Pokemon.

## Download and import it  
Go to [releases](https://github.com/oesiledivad/Pokedex-Anki/releases/latest) download the `.apkg` file open it and import it.  
Main deck is `Pokedex` it has subdecks by generations (1 to 9). If you dont wanna use subdecks, delete them and import the full `.csv` of your choice.  
Example:  
I want to use Español go to `csv` folder search `es` folder and download `pokedex_full_es.csv` import it, select the Note Type `Pokedex` and `Pokedex` deck import it and you should be good.


## Screenshots

#### Name

<div align="center" style="display: flex; align-items: center;">
  <img src="https://raw.githubusercontent.com/oesiledivad/Pokedex-Anki/refs/heads/main/screenshots/card1_1.png" height="auto" width="350" style="border-radius:20px;">
  <span style="font-size: 60px; margin: 0 15px;">&#8594;</span>
  <img src="https://raw.githubusercontent.com/oesiledivad/Pokedex-Anki/refs/heads/main/screenshots/card1_2.png" height="auto" width="350" style="border-radius:20px;">
</div>
</br>

---

#### Types

<div align="center" style="display: flex; align-items: center;">
  <img src="https://raw.githubusercontent.com/oesiledivad/Pokedex-Anki/refs/heads/main/screenshots/card2_1.png" height="auto" width="350" style="border-radius:20px;">
  <span style="font-size: 60px; margin: 0 15px;">&#8594;</span>
  <img src="https://raw.githubusercontent.com/oesiledivad/Pokedex-Anki/refs/heads/main/screenshots/card2_2.png" height="auto" width="350" style="border-radius:20px;">
</div>
</br>

----

#### Silhouette [type-in]

<div align="center" style="display: flex; align-items: center;">
  <img src="https://raw.githubusercontent.com/oesiledivad/Pokedex-Anki/refs/heads/main/screenshots/card3_1.png" height="auto" width="350" style="border-radius:20px;">
  <span style="font-size: 60px; margin: 0 15px;">&#8594;</span>
  <img src="https://raw.githubusercontent.com/oesiledivad/Pokedex-Anki/refs/heads/main/screenshots/card3_2.png" height="auto" width="350" style="border-radius:20px;">
</div>
</br>

----


#### Types [select]  
<div align="center" style="display: flex; align-items: center;">
  <img src="https://raw.githubusercontent.com/oesiledivad/Pokedex-Anki/refs/heads/main/screenshots/card4_1.png" height="auto" width="350" style="border-radius:20px;">
  <span style="font-size: 60px; margin: 0 15px;">&#8594;</span>
  <img src="https://raw.githubusercontent.com/oesiledivad/Pokedex-Anki/refs/heads/main/screenshots/card4_2.png" height="auto" width="350" style="border-radius:20px;">
</div>
</br>

<sup><em><strong>Working on AnkiDroid 2.19.beta3 and Anki Windows 24.06.3</strong></em></sup>

## Using other languages
If you want to use other languages, import `Pokedex_Anki.apkg`, delete all cards, import the `.csv` with the language you want.  

Now you'll need to modify `applyTypeColors()` in the `Front` part of all templates.

##### Instructions 
Here you have the Pokemon's [types](https://github.com/oesiledivad/Pokedex-Anki/tree/main/csv/_pkmn_types) in different languages. Now go to modify `Front` of the template and follow the example.  
Example:  
I want  to use French, go to `type_fr.csv` see what the english type name is in French. `Bug (English)` is `Insecte (French)` .  
Localize `applyTypeColors()`in the template and modify this variable `typesAndColors`.  
Default is english 

```javascript	
var typesAndColors = {
		electric: 'var(--electric-color)',
		water: 'var(--water-color)',
		grass: 'var(--grass-color)',
		ice: 'var(--ice-color)',
		fighting: 'var(--fighting-color)',
		poison: 'var(--poison-color)',
		ground: 'var(--ground-color)',
		flying: 'var(--flying-color)',
		psychic: 'var(--psychic-color)',
		bug: 'var(--bug-color)',
		rock: 'var(--rock-color)',
		ghost: 'var(--ghost-color)',
		dragon: 'var(--dragon-color)',
		dark: 'var(--dark-color)',
		steel: 'var(--steel-color)',
		fairy: 'var(--fairy-color)',
		fire: 'var(--fire-color)',
		normal: 'var(--normal-color)'
	};
   ```  
We follow `type_fr.csv` and replace all names (always lowercase) like this:  
   
```javascript	
var typesAndColors = {
		électrik: 'var(--electric-color)',
		eau: 'var(--water-color)',
		plante: 'var(--grass-color)',
		glace: 'var(--ice-color)',
		combat: 'var(--fighting-color)',
		poison: 'var(--poison-color)',
		sol: 'var(--ground-color)',
		vol: 'var(--flying-color)',
		psy: 'var(--psychic-color)',
		insecte: 'var(--bug-color)',
		roche: 'var(--rock-color)',
		spectre: 'var(--ghost-color)',
		dragon: 'var(--dragon-color)',
		ténèbres: 'var(--dark-color)',
		acier: 'var(--steel-color)',
		fée: 'var(--fairy-color)',
		feu: 'var(--fire-color)',
		normal: 'var(--normal-color)'
	};
   ```  
This should be done in all of `Front Card Types`. After doing this everything should work.
    

## Credits
[Sprites](https://www.spriters-resource.com/nintendo_switch/pokemonhome/)  
[PokeAPI](https://pokeapi.co/) for cries, other languages.  
[Font](https://www.dafont.com/pokemon-classic.font)  
Original idea by: /u/nunixnunix04  
Improvements and mass import by gleisonKZ and Akilez from Brazil  
I added generation 9  
