

- AppKit
- NSTextStorage
-  paragraphs 

Instance Property

# paragraphs

The text storage contents as an array of paragraphs.

macOS

``` source
var paragraphs: [NSTextStorage] { get set }
```

## Discussion

Unless you’re dealing with scriptability, you shouldn’t use or modify this property directly.

## See Also

### Accessing scriptable properties

var attributeRuns: [NSTextStorage]

The text storage contents as an array of attribute runs.

var words: [NSTextStorage]

The text storage contents as an array of words.

var characters: [NSTextStorage]

The text storage contents as an array of characters.

var font: NSFont?

The font for the text storage.

var foregroundColor: NSColor?

The color for the text.

