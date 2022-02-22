# Translation
Translating a plugin is really like how you translate TheoTown. The difference here is you will not use **.XML** for the values but you will used **JSON** instead. an exact example of these is how DSA translation are made here <a href="https://github.com/TheoTown-Team/translations/tree/master/dsa">See here</a>. Look up for available translation that the game supports <a href="https://github.com/TheoTown-Team/translations">here</a> so that your translation would appear if you changed the language in in-game settings.
 
# How translation works
Each <aos-values-xx.json> contains: **Array, Objects & Values** in the form of:
```json
[
  {
    "id": "hdst:aos-",
    "type": "translation",
    "X": {
      "IDS": "localized value",
      ...
    }
  }
]
```
while ```id``` is a unique identifier for this draft, you may used the format: "hdst:Aos-translation-X" with **X** is the <a href="">ISO 639-1<a> code of your country language. example: ```"id": "hdst:Aos-translation-en"``` as identifier for English translation.
