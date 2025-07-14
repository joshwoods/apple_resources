

- Foundation
- NSSpellServerDelegate
-  spellServer(\_:didLearnWord:inLanguage:) 

Instance Method

# spellServer(\_:didLearnWord:inLanguage:)

Notifies the delegate that the sender has added the specified word to the user’s list of acceptable words in the specified language.

Mac Catalyst 13.0+macOS 10.0+

``` source
optional func spellServer(
    _ sender: NSSpellServer,
    didLearnWord word: String,
    inLanguage language: String
)
```

## Parameters 

`sender`  

The `NSSpellServer` object that added the word.

`word`  

The word that was added.

`language`  

The language of the added word.

## Discussion

If your delegate maintains a similar auxiliary word list, you may wish to edit the list accordingly.

## See Also

### Managing the Spelling Dictionary

func spellServer(NSSpellServer, didForgetWord: String, inLanguage: String)

Notifies the delegate that the sender has removed the specified word from the user’s list of acceptable words in the specified language.

func spellServer(NSSpellServer, suggestCompletionsForPartialWordRange: NSRange, in: String, language: String) -> [String]?

This delegate method returns an array of possible word completions from the spell checker, based on a partially completed string and a given range.

func spellServer(NSSpellServer, recordResponse: Int, toCorrection: String, forWord: String, language: String)

Notifies the spell checker of the users’s response to a correction.

