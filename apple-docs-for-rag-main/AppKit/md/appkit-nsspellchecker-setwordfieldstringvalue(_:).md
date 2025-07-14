

- AppKit
- NSSpellChecker
-  setWordFieldStringValue(\_:) 

Instance Method

# setWordFieldStringValue(\_:)

Sets the string that appears in the misspelled word field, using the string object `aString`.

macOS

``` source
func setWordFieldStringValue(_ string: String)
```

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

func updateSpellingPanel(withMisspelledWord: String)

Causes the spell checker to update the Spelling panel’s misspelled-word field to reflect `word`.

func completions(forPartialWordRange: NSRange, in: String, language: String?, inSpellDocumentWithTag: Int) -> [String]?

Provides a list of complete words that the user might be trying to type based on a partial word in a given string.

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

