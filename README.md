# Fallen Starborn Translation
The repository of translations to the game Fallen Starborn by RKS Productions.

If you want to contribute to the project, this file will instruct you to how send your translation, but, the translation can be easier entering to the  [Community Discord](https://discord.gg/JBeh9Ampy3), so you can contact others translators, and even RKS (Game Developer). once in the server, go to Fallen Starborn's Category and react the contribution message in the `translation` channel, pick your translation role in the `pick-role` channel.

> [!WARNING]
> all original translation files (english) may change their content, thus requiring a revision or even being redone entirely, and every time these changes are made, RKS (`@5rks`) will notify you on the discord server in the contributors channel. So if you don't have the patience to revise or redo the entire translation, wait until RKS gives notice that this is the last change and that one will be kept for the final game.

## Translating correctly the texts of Fallen Starborn
### Organization of the main translation file
The file of translation is a `.csv` archive, that is a spreadsheet separeted by comma. You can use any app/site to create your translations. I particularly recommend [Google Sheets](https://docs.google.com/spreadsheets).
- **First column** - Here is where the **keys** are located. They are the "name" of the text. For example, if the game is trying to write the option to start the game, it will pull the `ini_ng` key, and when you run the game in English, the text "New game" will appear on the screen, or if you run the game in Portuguese, "Novo jogo" will appear, and so on. The first line must be written "Keys", just to standardize;
- **Second column** - Here is the translated texts, with always the first line being the name of the language (on the way it's written in their own language, that text is used to identify the language in the language option of the settings);
- You just need to have these 2 columns, keys and language, respectively. If you want to have annotations about the translation, both to remember preferences in translation, observations, or to guide other translators of that language, you can create a new file (called [`abbreviation of the language`](https://www.loc.gov/standards/iso639-2/php/English_list.php) + [`abbreviation of the country in capital`](https://www.iban.com/country-codes) + `_notes.txt`, `_notes.odt` or any type of text file)
- If you want to translate more languages, you have to create another file to your other translation.

### Workflow
- If you want to test the translation in-game, just put your translation file in the languages file of the game (`...game directory\langs`), the game has a system that auto-identify the translations files, so just run the game and select your translating language in the settings.
- If the language you're translating uses characters differents of the latin script ones (such as those used in English or Portuguse), let RKS (`@5rks`) know on the game server which language you're translating into, and he will add support for that language to the game as quickly as he can.

### Code words
In the spreadsheet of translation, you going to see some strange words/codes, here are the explication and usage of all of them.
- **`{0}, {1}, {2}...`** - This is a word of replacement, for texts in which parts of it can change depending on the context in game. For example, the key `uti_desc_000_003` returns "Grants {0} Shards." this `{0}` will be replaced by the amount of Shards (game's currency) that item give.
- **`[n]`** - Line break code. This is used to go to the next line.

### Text Variations
- In some moments of the translation you will see the keys with almost the same name, but with the suffix `m_one`, `f_one`, `m_two` or `f_two`. Those are inflections of the noun, such as in gender (masculine or feminine) or number (singular, plural, etc.). `m_one`: singular masculine; `f_one`: singular feminine; `m_two`: plural masculine; `f_two`: plural feminine.
- There may also be keys with only gender or number inflection, like `_m`, `_f`, or `_one`, `_two`, `_few`, `_many` and `_other`.
- These number inflections may differ a lot in each language, so check out the [Language Plural Rules Document](https://www.unicode.org/cldr/charts/43/supplemental/language_plural_rules.html) to get a better understanding of how each one works in your language.

### Proper names
Here is the list of proper names of areas, characters, items, etc. I prefer that you just transliterate them. If there are any problems with the translation, such as names meaning something wrong or nasty in your language, or some kind of double entendre, please contact RKS (@5rks) on Discord to discuss a good adaptation for these name.
- Vehord — Lupine Lord, Lord of the Night and final boss of the game, a powerful giant black wolf.
- Bonyare — First optional boss of the game, a great ogre-wolf red beast.
- Lentrard — Second optional boss of the game, a giant three-headed skeleton shaman.
- Fugnarg — third optional boss of the game.
- Yonagi — Boss necessary to enter Vehord Domain.
- Gothye Hankyrd — Great cleric highly renowned. Creator of the Jernika Church, its Sanctuaries and Gotyhe's Enchant.
- Enpharism — Most followed religion of the game, based on Irish mythology.
- Cxauo — One of the game's religions, based on Shintoism.
- Veoethism — One of the game's religion, based on Hinduism
- Jernika — Enpharism's Goddess of life, Mother Goddess, All-Mother.
- Tsukare — Cxuao's Goddess of nature and fertility.
- Hsurd — Veoethism's God of mischief and fun
- Gishanu — Veoethism's God of Prosperity and Knowledge.
- Yrgvonia — Human kingdom inspired in China, destroyed by the Firrelins.
- Firrelin — The legion of demons and beasts of the Cerulean Stars.
- Coitiant — Werewolf-like Firrelin.
- Aureliph — Black Bear-like Firrelin.
- Dorclave — Giant bat-like Firrelin.
- Lubgurn — United Firrelins melted into slime.
- Lugnarph — Demon goat-like Firrelin.
- Varnake — Primate-like Firrelin.

## Other files
**Achievements**
- This is the translation file for the game's achievements on Steam.
- The `“language”` field must have the name of the language written in English.
- Inside the second braces is the list of names (`ACH` + Achievement number + `_NAME`) and descriptions (`ACH` + Achievement number + `_DESC`) of the achievements. The first field are the translation keys, so do not change them, and the translation should be in the second field.

**Steam**
- This is the translation file for the game's Steam page.
- There are two texts, the "Short description", that little texts that appears on the top right of the game's Steam page, like a synopsis, and the "About this game", the long description that says about every aspect of the game. Weird codes (like `[h2][/h2]` or `[b][/b]`) are text formatting, such as titles, bold, italics, etc. Don't worry about it, just put them in the same words as the original text.

## Send the translation to the repository
1. Download the [`enUS.csv`](https://github.com/5RKS/Fallen-Starborn-Translation/blob/main/enUS.csv) and translate all the text to the language that you want to translate the game.
<img width="1574" height="313" alt="image" src="https://github.com/user-attachments/assets/456d723e-dd0e-4ef8-9080-2c32c898d8ed" />

2. After changing the archive for entire to the language that you want to translate the game, return to the repository and click on `add files` and then `create new file`.
<img width="936" height="317" alt="image" src="https://github.com/user-attachments/assets/e9269014-d0c1-437a-8b48-bb64a2773904" />

3. Create a new fork.
<img width="820" height="228" alt="image" src="https://github.com/user-attachments/assets/6da4d664-4775-484d-9b5e-bf58ae46fd79" />

4. Name the file the [`abbreviation of the language`](https://www.loc.gov/standards/iso639-2/php/English_list.php) + [`abbreviation of the country in capital`](https://www.iban.com/country-codes) + `.csv`, like `ptPT.csv` for the Portuguese of Portugal translation, for example.
<img width="584" height="201" alt="image" src="https://github.com/user-attachments/assets/dcf6720a-4062-42ac-be96-39fd15d090c5" />

5. Save the file that you translated as `.csv` wherever you want, open the `.csv` and copy all (``Ctrl+A`` and then ``Ctrl+C``).
<img width="631" height="495" alt="image" src="https://github.com/user-attachments/assets/40f2df5d-2497-43ff-93e8-a8569013684a" />

6. Paste on the file (`Ctrl+V`) you are creating on GitHub.
<img width="615" height="346" alt="image" src="https://github.com/user-attachments/assets/2408c570-3d6a-4df8-98b9-ba1de1fdcf2a" />

7. Click on `Commit changes...`.
<img width="398" height="176" alt="image" src="https://github.com/user-attachments/assets/2cca9b90-094d-47fa-a354-1e0a724bf893" />

8. Create a name and description to the propose, making it clear that this is a translation propose, and remember to include how you want your name to appear in the game credits (if you have already written how you want your name to appear in another pull request, you don't need to include it in this one, unless you want a change it, in which case you can tell RKS directly on Discord), and click on `Propose changes`.
<img width="495" height="448" alt="image" src="https://github.com/user-attachments/assets/2302312c-26df-41ca-98b3-603cc92634aa" />

9. Now click on `Create pull request`.
<img width="1243" height="491" alt="image" src="https://github.com/user-attachments/assets/58e7c27b-482f-49d0-94cf-cbce99642aff" />

10. Click again on `Create pull request`.
<img width="1243" height="491" alt="image" src="https://github.com/user-attachments/assets/fc30eb0d-9079-4969-9f88-f37ef582e7a5" />

11. And for the last time, click on `Create pull request`.
<img width="925" height="585" alt="image" src="https://github.com/user-attachments/assets/c0710e40-462d-4c61-b0a9-31433eb7375f" />

And it's done. Wait for RKS approve or reject your pull request, if you want, you can ping him (`@5rks`) in "translation-chat" on Discord, probably he will see your pull request much faster.

## FAQ
### 1. Why do some texts have quotation marks at the beginning and end, but others don't? (if you are using a spreadsheet editor, don't worry about this block, it's only noticeable when using a text editor)
`.csv` archives works with commas, so if the text have commas, you need to put that whole text in quotation marks, so that the file doesn't identify it as another text. So while you're editing texts, always remember to put those with commas in quotation marks, or put all the texts in quotation marks, it also works.

### 2. How do I know which texts have been changed, added or deleted?
In the repository commits, when you click on the commit you want to analyze, you can see the changes of the files, where you can see the changes, additions or deletions.
