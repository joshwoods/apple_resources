

- AppKit
- NSSpellChecker
-  completions(forPartialWordRange:in:language:inSpellDocumentWithTag:) 

Instance Method

# completions(forPartialWordRange:in:language:inSpellDocumentWithTag:)

Provides a list of complete words that the user might be trying to type based on a partial word in a given string.

macOS

``` source
func completions(
    forPartialWordRange range: NSRange,
    in string: String,
    language: String?,
    inSpellDocumentWithTag tag: Int
) -> [String]?
```

## Parameters 

`range`  

Range that identifies a partial word in `string`.

`string`  

String with the partial word from which to generate the result.

`language`  

Language to used in `string`. When `nil`, this method uses the language selected in the Spelling panel.

`tag`  

Identifies the spell document with ignored words to use.

## Return Value

List of complete words from the spell checker dictionary in the order they should be presented to the user.

## See Also

### Managing the Spell-Checking Process

class func uniqueSpellDocumentTag() -> Int

Returns a guaranteed unique tag to use as the spell-document tag for a document.

func closeSpellDocument(withTag: Int)

Notifies the receiver that the user has finished with the tagged document.

func ignoreWord(String, inSpellDocumentWithTag: Int)

Instructs the spell checker to ignore all future occurrences of `wordToIgnore` in the document identified by `tag`.

func ignoredWords(inSpellDocumentWithTag: Int) -> [String]?

Returns the array of ignored words for a document identified by `tag`.

func setIgnoredWords([String], inSpellDocumentWithTag: Int)

Initializes the ignored-words document (a dictionary identified by `tag` with `someWords`), an array of words to ignore.

func setWordFieldStringValue(String)

Sets the string that appears in the misspelled word field, using the string object `aString`.

func updateSpellingPanel(withMisspelledWord: String)

Causes the spell checker to update the Spelling panel’s misspelled-word field to reflect `word`.

func hasLearnedWord(String) -> Bool

Indicates whether the spell checker has learned a given word.

func unlearnWord(String)

Tells the spell checker to unlearn a given word.

func learnWord(String)

Adds the word to the spell checker dictionary.

func userQuotesArray(forLanguage: String) -> [String]

Returns the default values for quote replacement.

var userReplacementsDictionary: [String : String]

Returns the dictionary used when replacing words.

