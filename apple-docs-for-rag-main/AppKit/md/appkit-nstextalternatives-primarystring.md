

- AppKit
- NSTextAlternatives
-  primaryString 

Instance Property

# primaryString

The text that was initially chosen as the input string.

macOS 10.8+

``` source
var primaryString: String { get }
```

## Discussion

The text system uses the `primaryString` property to make sure that the text is still in the same state as when it was entered.

## See Also

### Storing Alternative Text Strings

var alternativeStrings: [String]

An array of alternative possible interpretations that the user might select.

