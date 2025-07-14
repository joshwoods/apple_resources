

- AppKit
- NSChangeSpelling
-  changeSpelling(\_:) 

Instance Method

# changeSpelling(\_:)

Replaces the selected word in the receiver with a corrected version from the Spelling panel.

macOS

``` source
func changeSpelling(_ sender: Any?)
```

**Required**

## Discussion

This message is sent by the `NSSpellChecker` to the object whose text is being checked. To get the corrected spelling, ask `sender` for the string value of its selected cell (visible to the user as the text field in the Spelling panel). This method should replace the selected portion of the text with the string that it gets from the NSSpellChecker.

## See Also

### Related Documentation

Spell Checking Programming Topics

