# TUD translations!
Use this guide to add translation files for the Time Use Diary feature. Translation files are organized by language code. For example, English translation file is stored in **en/translation.json**.  For a complete list of language codes, please visit http://www.lingoes.net/en/translator/langcode.htm

## Adding a new language translation
To add a new translation:

 1.  Clone the project repository: `git clone https://github.com/anzioka/translations-demo.git`
 2. Navigate to the root of the project (`translations-demo`)
 3. Create a new branch. Example `git checkout task/add-german-translation`
 4. Create a new folder with name matching the language code. For example, German would require a **de** folder.
 5. Copy over the **translation.json** file from the **en** folder to the new folder.
 6. The translation.json file has a `key: value` format. Replace all the `value`s with the appropriate translation. **Please do not modify any text surrounded by {{ }} brackets.**
 For example: `typical_day: was yesterday a typical {{day}} for you.`  In this case you would translate all the text except `{{day}}`.

 8. Commit and push changes. For example `git add`, then `git commit -m "add German translations"`. Finally, `git push --set-upstream origin task/add-german-translation`
 9. Create a pull request
