

- AppKit
- NSTextStorage
-  font 

Instance Property

# font

The font for the text storage.

macOS

``` source
var font: NSFont? { get set }
```

## Discussion

Unless you’re dealing with scriptability, you shouldn’t use or modify this property directly.

## See Also

### Accessing scriptable properties

var attributeRuns: [NSTextStorage]

The text storage contents as an array of attribute runs.

var paragraphs: [NSTextStorage]

The text storage contents as an array of paragraphs.

var words: [NSTextStorage]

The text storage contents as an array of words.

var characters: [NSTextStorage]

The text storage contents as an array of characters.

var foregroundColor: NSColor?

The color for the text.

