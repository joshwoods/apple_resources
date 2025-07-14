

- AppKit
- NSRuleEditor
-  formattingDictionary 

Instance Property

# formattingDictionary

The formatting dictionary for the rule editor.

macOS

``` source
@MainActor
var formattingDictionary: [String : String]? { get set }
```

## Discussion

If you assign a new the formatting dictionary to this property, it sets the current to formatting strings file name to `nil`.

## See Also

### Working with Formatting

var formattingStringsFilename: String?

The name of the rule editor’s strings file.

