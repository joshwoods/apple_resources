

- AppKit
- NSIgnoreMisspelledWords
-  ignoreSpelling(\_:) 

Instance Method

# ignoreSpelling(\_:)

macOS

``` source
func ignoreSpelling(_ sender: Any?)
```

**Required**

## Discussion

Implement this action method to allow an application to ignore misspelled words on a document-by-document basis. This message is sent by the NSSpellChecker instance to the object whose text is being checked.

Implement this method by using the code shown in the protocol description.

## See Also

### Related Documentation

Spell Checking Programming Topics

