# Translation
Translating a plugin is really like how you translate TheoTown. The difference here is you will not use **.XML** for the values but you will used **JSON** instead. an exact example of these is how DSA translation are made here <a href="https://github.com/TheoTown-Team/translations/tree/master/dsa">See here</a>. Look up for available translation that the game supports <a href="https://github.com/TheoTown-Team/translations">here</a> so that your translation would appear if you changed the language in in-game settings.
 
# How translation works
Each <aos-values-xx.json> contains: **Array, Objects & Values** in the form of:
```json
[
  {
    "id": "hdst:aos-translation-X",
    "type": "translation",
    "X": {
      "IDS": "localized value"

    }
  }
]
```
### Parts
```id``` is a unique identifier for this draft, you may use the format: ```"id": "hdst:aos-translation-X"``` while **X** is the <a href="http://www.loc.gov/standards/iso639-2/php/code_list.php">ISO 639-1<a> language code. example: ```"id": "hdst:aos-translation-fil"``` as identifier for Filipino language.
 
 ```type``` the type of the draft, values should always be: ```"translation"```
 
 ```X``` the **ISO 639-1** code of your language, (e.g. ```"fil": {}```)for Filipino language.
 
 ```IDS``` are the translation value of each drafts inside the plugin, **These are all constant**. kindly check "aos-values-en.json" for id's value.


```localized value``` the corresponding translation of your language.
 
**Please check out "aos-values-en.json" as reference. and also don't forget JSON syntax**
 
Special characters like \n might be used to indicate a new line.
If you see any characters like ```${$aos-planks}``` it is a variable for integers so leave it as it is.

 
 When your translation is done, make sure to create a 'pull request' so it can be merged to main branch. If you forget to do that step your translation won't be added to the main branch.
