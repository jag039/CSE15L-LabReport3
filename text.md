# Lab Report 3
Jesus Gonzalez - CSE 15L - A17425808 - Feb 12, 2023

## find command
---
### grep -c
The grep can report the number of times that the pattern has been matched for each file using -c (count) option:

```
grep -r -c Lucayans skill-demo1-data/written_2/travel_guides/berlitz2
skill-demo1-data/written_2/travel_guides/berlitz2/Algarve-History.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Algarve-Intro.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Algarve-WhatToDo.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Algarve-WhereToGo.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Amsterdam-History.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Amsterdam-Intro.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Amsterdam-WhatToDo.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Amsterdam-WhereToGo.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Athens-History.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Athens-Intro.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Athens-WhatToDo.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Athens-WhereToGo.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Bahamas-History.txt:2
.........(shows all files in directory
```
There are 2 occurances of the string "Lucayans" in the fle Bahamas-History.txt

```
grep -r -c Paris skill-demo1-data/written_2/travel_guides/berlitz2
skill-demo1-data/written_2/travel_guides/berlitz2/Algarve-History.txt:1
skill-demo1-data/written_2/travel_guides/berlitz2/Algarve-Intro.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Algarve-WhatToDo.txt:1
skill-demo1-data/written_2/travel_guides/berlitz2/Algarve-WhereToGo.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Amsterdam-History.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Amsterdam-Intro.txt:1
skill-demo1-data/written_2/travel_guides/berlitz2/Amsterdam-WhatToDo.txt:1
skill-demo1-data/written_2/travel_guides/berlitz2/Amsterdam-WhereToGo.txt:2
skill-demo1-data/written_2/travel_guides/berlitz2/Athens-History.txt:1
skill-demo1-data/written_2/travel_guides/berlitz2/Athens-Intro.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Athens-WhatToDo.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Athens-WhereToGo.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Bahamas-History.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Bahamas-Intro.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Bahamas-WhatToDo.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Bahamas-WhereToGo.txt:1
skill-demo1-data/written_2/travel_guides/berlitz2/Bali-History.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Bali-WhatToDo.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Bali-WhereToGo.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Barcelona-History.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Barcelona-WhatToDo.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Barcelona-WhereToGo.txt:2
skill-demo1-data/written_2/travel_guides/berlitz2/Beijing-History.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Beijing-WhatToDo.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Beijing-WhereToGo.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Berlin-History.txt:2
skill-demo1-data/written_2/travel_guides/berlitz2/Berlin-WhatToDo.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Berlin-WhereToGo.txt:3
skill-demo1-data/written_2/travel_guides/berlitz2/Bermuda-WhatToDo.txt:7
skill-demo1-data/written_2/travel_guides/berlitz2/Bermuda-WhereToGo.txt:4
skill-demo1-data/written_2/travel_guides/berlitz2/Bermuda-history.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Boston-WhereToGo.txt:1
skill-demo1-data/written_2/travel_guides/berlitz2/Budapest-History.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Budapest-WhatToDo.txt:2
skill-demo1-data/written_2/travel_guides/berlitz2/Budapest-WhereoGo.txt:3
skill-demo1-data/written_2/travel_guides/berlitz2/California-History.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/California-WhatToDo.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/California-WhereToGo.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Canada-History.txt:1
skill-demo1-data/written_2/travel_guides/berlitz2/Canada-WhereToGo.txt:3
skill-demo1-data/written_2/travel_guides/berlitz2/CanaryIslands-History.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/CanaryIslands-WhatToDo.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/CanaryIslands-WhereToGo.txt:1
skill-demo1-data/written_2/travel_guides/berlitz2/Cancun-History.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Cancun-WhatToDo.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Cancun-WhereToGo.txt:1
skill-demo1-data/written_2/travel_guides/berlitz2/China-History.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/China-WhatToDo.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/China-WhereToGo.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Costa-History.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Costa-WhatToDo.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Costa-WhereToGo.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/CostaBlanca-History.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/CostaBlanca-WhatToDo.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Crete-History.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Crete-WhatToDo.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Crete-WhereToGo.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/CstaBlanca-WhereToGo.txt:1
skill-demo1-data/written_2/travel_guides/berlitz2/Cuba-History.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Cuba-WhatToDo.txt:2
skill-demo1-data/written_2/travel_guides/berlitz2/Cuba-WhereToGo.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Nepal-History.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Nepal-WhatToDo.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Nepal-WhereToGo.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/NewOrleans-History.txt:0
skill-demo1-data/written_2/travel_guides/berlitz2/Paris-WhatToDo.txt:14
skill-demo1-data/written_2/travel_guides/berlitz2/Paris-WhereToGo.txt:44
```

---
### grep -i
The -i addon performs a case-insensitive search for the word following. This is usefull because maybe you want to search for all occurences of a word, not just the ones capatalized or the ones lowercased.

```
grep -c -i nothing skill-demo1-data/written_2/travel_guides/berlitz2/Paris-WhereToGo.txt

2
```

```
grep -c  nothing skill-demo1-data/written_2/travel_guides/berlitz2/Paris-WhereToGo.txt

1
```
These two examples show the count of the string Nothing in the file with and without the -i addon. This means that -i addon allows the grep command to search for the string without worry about the casetype of the characters in the String.
```
grep -i  nothing skill-demo1-data/written_2/travel_guides/berlitz2/Paris-WhereToGo.txt

Their anxiety is nothing compared with that of the prisoners once held in the forbidding Conciergerie (entrance on the quai de l’Horloge). It was originally the residence of the king’s concierge as part of the 14th-century royal palace. In 1793, at the height of the Terror, it literally became the “antechamber of the guillotine.” Queen Marie-Antoinette, Robespierre, Danton, and Saint-Just all spent their last nights in the Galerie des Prisonniers. The Salle des Girondins displays a guillotine blade, the crucifix to which Marie-Antoinette prayed, and the lock used on Robespierre’s cell. Look out on the Cour des Femmes, where husbands, lovers, wives, and mistresses were allowed one final tryst before the tumbrels came to carry off the condemned. About 2,500 victims of the Revolutionary guillotine spent their last hours in the Conciergerie.
Take the métro to Rambuteau and start at the corner of the rue des Archives and the rue des Francs-Bourgeois, named after the poor (not bourgeois at all) allowed to live here tax-free in the 14th century. The national archives are stored in an 18th-century mansion, Hôtel de Soubise. Across a vast, horseshoe-shaped courtyard, you come across the exquisite Rococo style of Louis XV’s time in the apartments of the Prince and Princess of Soubise. Up on the first floor is the Musée de l’Histoire de France, with gems such as the only known portrait of Joan of Arc painted in her lifetime and the diary kept by Louis XVI. His entry for 14 July 1789, the day the Bastille was stormed, reads Rien (Nothing).
```
When justing using grep -i, the part of the file containg the matched string is returned.

###



