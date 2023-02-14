# Lab Report 3
Jesus Gonzalez - CSE 15L - A17425808 - Feb 12, 2023

## grep command
(source)[https://www.cyberciti.biz/faq/howto-use-grep-command-in-linux-unix/]
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
The -c addon shows the amount of occurnces of the String paris in all files in the directory.

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

---
### grep -n
Pass the -n option to precede each line of output with the number of the line in the text file from which it was obtained. It is usefull to find out where in the file the search words actually are.
```
grep -r -n Lucayans skill-demo1-data/written_2/travel_guides/berlitz2

skill-demo1-data/written_2/travel_guides/berlitz2/Bahamas-History.txt:6:Centuries before the arrival of Columbus, a peaceful Amerindian people who called themselves the Luccucairi had settled in the Bahamas. Originally from South America, they had traveled up through the Caribbean islands, surviving by cultivating modest crops and from what they caught from sea and shore. Nothing in the experience of these gentle people could have prepared them for the arrival of the Pinta, the Niña, and the Santa Maria at San Salvador on 12 October 1492. Columbus believed that he had reached the East Indies and mistakenly called these people Indians. We know them today as the Lucayans. Columbus claimed the island and others in the Bahamas for his royal Spanish patrons, but not finding the gold and other riches he was seeking, he stayed for only two weeks before sailing towards Cuba.

skill-demo1-data/written_2/travel_guides/berlitz2/Bahamas-History.txt:7:The Spaniards never bothered to settle in the Bahamas, but the number of shipwrecks attest that their galleons frequently passed through the archipelago en route to and from the Caribbean, Florida, Bermuda, and their home ports. On Eleuthera the explorers dug a fresh-water well — at a spot now known as “Spanish Wells” — which was used to replenish the supplies of water on their ships before they began the long journey back to Europe with their cargoes of South American gold. As for the Lucayans, within 25 years all of them, perhaps some 30,000 people, were removed from the Bahamas to work — and die — in Spanish gold mines and on farms and pearl fisheries on Hispaniola (Haiti), Cuba, and elsewhere in the Caribbean.
```
The first occurence of the string "Lucayans" is in the Bahamas-history.txt line 6 and line 7.
```
grep -r -n Nothing skill-demo1-data/written_2/travel_guides/berlitz2

skill-demo1-data/written_2/travel_guides/berlitz2/Bahamas-History.txt:6:Centuries before the arrival of Columbus, a peaceful Amerindian people who called themselves the Luccucairi had settled in the Bahamas. Originally from South America, they had traveled up through the Caribbean islands, surviving by cultivating modest crops and from what they caught from sea and shore. Nothing in the experience of these gentle people could have prepared them for the arrival of the Pinta, the Niña, and the Santa Maria at San Salvador on 12 October 1492. Columbus believed that he had reached the East Indies and mistakenly called these people Indians. We know them today as the Lucayans. Columbus claimed the island and others in the Bahamas for his royal Spanish patrons, but not finding the gold and other riches he was seeking, he stayed for only two weeks before sailing towards Cuba.

skill-demo1-data/written_2/travel_guides/berlitz2/Bali-WhereToGo.txt:162:Practically every brochure for Bali shows this exotic sea temple on its rocky islet, often silhouetted against the setting sun. Inevitably, tour buses converge here in late afternoon so everyone can take that same picture. It is 10 km (6 miles) down a narrow side road from Kediri to the coast, and there can be a long procession of traffic. You might like to plan a dawn visit instead, avoiding at least some of the hawkers who congregate later in the day. Tanah Lot is believed to have been founded in the 16th century by the Javanese priest Nirarta, who dedicated it to the sea god. Now the sea threatens to undermine the rock on which it stands, and concrete breakwaters have been positioned to hold back the waves. Nothing, however, is done to hold back the commercial tide. Ever more souvenir stands and food stalls cluster as near as they can get, and the nearby coast is being developed as a huge, and controversial, resort complex.

skill-demo1-data/written_2/travel_guides/berlitz2/Boston-WhereToGo.txt:101:Nothing in Boston can match the beauty of the courtyard in the Isabella Stewart Gardner Museum. Modeled on a Venetian loggia, the cloister, delicate arches, and salmon-pink marble walls enclose a stunning, atmospheric space lined with mosaic and filled with foliage and classical statuary. Isabella Gardner created Fenway Court in 1903 to hold her outstanding collection of art. A flamboyant New Yorker, her unconventional ways scandalized the Boston Brahmins on more than one occasion. Her portrait by John Singer Sargent (in the Gothic Room) captures her individuality and her eccentricity lives on in her will, which stipulates that all of the 2,000 pieces on display in the house must be left exactly where they are. This decree is qualified by the condition that were anything to change, the museum’s contents would be sold off, with the proceeds going to Harvard University. It’s an extraordinary place filled with great art works which are displayed idiosyncratically in often (for the time) innovative ways. It’s more a personal home than a museum and the works are often poorly lit and cursorily labeled. Each of the rooms displays art of a particular artist — Titian, Raphael, or Veronese — or style — Dutch, Gothic, or early Italian.

skill-demo1-data/written_2/travel_guides/berlitz2/CostaBlanca-History.txt:6:Nothing has had a greater impact on the Costa Blanca than foreign invasion: Iberians, Phoenicians, Greeks, Romans, Visigoths, and Moors had moulded Spain’s Mediterranean shores centuries before international tourism gained a foothold. But before any of these were the Costa Blanca’s first inhabitants: Known as Neanderthal men, they lived primitively and spent a large part of their time hunting. Then, as the Stone Age came to an end, short, dark-skinned Iberians started to make their way from North Africa to the Spanish Peninsula. These fierce fighters skilled in guerrilla warfare roamed the Mediterranean foothills, painting a vivid record of their battles on the walls of their rock shelters.

skill-demo1-data/written_2/travel_guides/berlitz2/Paris-WhereToGo.txt:84:Take the métro to Rambuteau and start at the corner of the rue des Archives and the rue des Francs-Bourgeois, named after the poor (not bourgeois at all) allowed to live here tax-free in the 14th century. The national archives are stored in an 18th-century mansion, Hôtel de Soubise. Across a vast, horseshoe-shaped courtyard, you come across the exquisite Rococo style of Louis XV’s time in the apartments of the Prince and Princess of Soubise. Up on the first floor is the Musée de l’Histoire de France, with gems such as the only known portrait of Joan of Arc painted in her lifetime and the diary kept by Louis XVI. His entry for 14 July 1789, the day the Bastille was stormed, reads Rien (Nothing).
```
In this example the grep -r recursively searches through all the files in the directory, and returns the (-n) the line number where the word is, along with the line.
---
### grep -l
Use the -l option to list the file name whose contents mention the string
```
grep -r -l Nothing skill-demo1-data

skill-demo1-data/written_2/non-fiction/OUP/Berk/CH4.txt
skill-demo1-data/written_2/non-fiction/OUP/Berk/ch7.txt
skill-demo1-data/written_2/non-fiction/OUP/Fletcher/ch1.txt
skill-demo1-data/written_2/non-fiction/OUP/Kauffman/ch6.txt
skill-demo1-data/written_2/non-fiction/OUP/Rybczynski/ch1.txt
skill-demo1-data/written_2/non-fiction/OUP/Rybczynski/ch2.txt
skill-demo1-data/written_2/travel_guides/berlitz1/HistoryFrance.txt
skill-demo1-data/written_2/travel_guides/berlitz1/HistoryIndia.txt
skill-demo1-data/written_2/travel_guides/berlitz1/WhatToJapan.txt
skill-demo1-data/written_2/travel_guides/berlitz1/WhatToLasVegas.txt
skill-demo1-data/written_2/travel_guides/berlitz1/WhereToFrance.txt
skill-demo1-data/written_2/travel_guides/berlitz1/WhereToItaly.txt
skill-demo1-data/written_2/travel_guides/berlitz1/WhereToLosAngeles.txt
skill-demo1-data/written_2/travel_guides/berlitz2/Bahamas-History.txt
skill-demo1-data/written_2/travel_guides/berlitz2/Bali-WhereToGo.txt
skill-demo1-data/written_2/travel_guides/berlitz2/Boston-WhereToGo.txt
skill-demo1-data/written_2/travel_guides/berlitz2/CostaBlanca-History.txt
skill-demo1-data/written_2/travel_guides/berlitz2/Paris-WhereToGo.txt
```
The -l option here shows all the files within the directory that contain the string "Nothing"

```
grep -r -l Lucayans skill-demo1-data
skill-demo1-data/written_2/travel_guides/berlitz2/Bahamas-History.txt
```
Here the -l option shows the only file that contains the string Lucayans.




