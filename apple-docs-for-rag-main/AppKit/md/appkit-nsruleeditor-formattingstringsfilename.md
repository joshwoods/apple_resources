

- AppKit
- NSRuleEditor
-  formattingStringsFilename 

Instance Property

# formattingStringsFilename

The name of the rule editor’s strings file.

macOS

``` source
@MainActor
var formattingStringsFilename: String? { get set }
```

## Discussion

The `NSRuleEditor` class looks for a strings file with the given name in the main bundle and (if appropriate) the bundle containing the nib file from which it was loaded. If it finds a strings file resource with the given name, `NSRuleEditor` loads it and sets it as the formatting dictionary for the receiver. You can obtain the resulting dictionary using the formattingDictionary property\].

If you assign a new dictionary to the formattingDictionary property, it sets the current to formatting strings file name to `nil`.

## See Also

### Working with Formatting

var formattingDictionary: [String : String]?

The formatting dictionary for the rule editor.

