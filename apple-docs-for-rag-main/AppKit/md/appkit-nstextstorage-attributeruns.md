

- AppKit
- NSTextStorage
-  attributeRuns 

Instance Property

# attributeRuns

The text storage contents as an array of attribute runs.

macOS

``` source
var attributeRuns: [NSTextStorage] { get set }
```

## Discussion

Unless you’re dealing with scriptability, you shouldn’t use or modify this property directly.

## See Also

### Accessing scriptable properties

var paragraphs: [NSTextStorage]

The text storage contents as an array of paragraphs.

var words: [NSTextStorage]

The text storage contents as an array of words.

var characters: [NSTextStorage]

The text storage contents as an array of characters.

var font: NSFont?

The font for the text storage.

var foregroundColor: NSColor?

The color for the text.

