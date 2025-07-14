

- AppKit
- NSTextAlternatives
-  alternativeStrings 

Instance Property

# alternativeStrings

An array of alternative possible interpretations that the user might select.

macOS 10.8+

``` source
var alternativeStrings: [String] { get }
```

## Discussion

The text system presents the alternative strings via a user interface similar to that used for spelling correction alternatives.

## See Also

### Storing Alternative Text Strings

var primaryString: String

The text that was initially chosen as the input string.

