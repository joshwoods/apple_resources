

- Foundation
- NSSpellServerDelegate
-  spellServer(\_:suggestCompletionsForPartialWordRange:in:language:) 

Instance Method

# spellServer(\_:suggestCompletionsForPartialWordRange:in:language:)

This delegate method returns an array of possible word completions from the spell checker, based on a partially completed string and a given range.

Mac Catalyst 13.0+macOS 10.0+

``` source
optional func spellServer(
    _ sender: NSSpellServer,
    suggestCompletionsForPartialWordRange range: NSRange,
    in string: String,
    language: String
) -> [String]?
```

## Parameters 

`sender`  

The `NSSpellServer` object that sent this message.

`range`  

The range of the partially completed word.

`string`  

The string containing the partial word range.

`language`  

The language to use for the completion.

## Return Value

An array of `NSString` objects indicating possible completions.

## See Also

### Related Documentation

func completions(forPartialWordRange range: NSRange, in string: String, language: String?, inSpellDocumentWithTag tag: Int) -> [String]?

Provides a list of complete words that the user might be trying to type based on a partial word in a given string.

### Managing the Spelling Dictionary

func spellServer(NSSpellServer, didForgetWord: String, inLanguage: String)

Notifies the delegate that the sender has removed the specified word from the user’s list of acceptable words in the specified language.

func spellServer(NSSpellServer, didLearnWord: String, inLanguage: String)

Notifies the delegate that the sender has added the specified word to the user’s list of acceptable words in the specified language.

func spellServer(NSSpellServer, recordResponse: Int, toCorrection: String, forWord: String, language: String)

Notifies the spell checker of the users’s response to a correction.

