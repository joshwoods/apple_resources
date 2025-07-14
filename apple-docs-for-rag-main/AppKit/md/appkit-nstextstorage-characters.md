

- AppKit
- NSTextStorage
-  characters 

Instance Property

# characters

The text storage contents as an array of characters.

macOS

``` source
var characters: [NSTextStorage] { get set }
```

## Discussion

Unless you’re dealing with scriptability, you shouldn’t use or modify this property directly. For indexed access to characters, use `NSAttributedString`’s length method to access the string, and `NSString`’s character(at:) method to access the individual characters.

## See Also

### Accessing scriptable properties

var attributeRuns: [NSTextStorage]

The text storage contents as an array of attribute runs.

var paragraphs: [NSTextStorage]

The text storage contents as an array of paragraphs.

var words: [NSTextStorage]

The text storage contents as an array of words.

var font: NSFont?

The font for the text storage.

var foregroundColor: NSColor?

The color for the text.

