

- Foundation
- AttributedStringProtocol
-  unicodeScalars 

Instance Property

# unicodeScalars

The Unicode scalars of the attributed string, as a view into the underlying string.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var unicodeScalars: AttributedString.UnicodeScalarView { get }
```

**Required**

## Discussion

Use this property when you want to split the attributed string by Unicode scalar instead of grapheme cluster. This is useful when you need to carefully control insertion points or render the content.

You can also use this property to mutate the attributed string, using RangeReplaceableCollection methods, such as `insert(_:at:)` and append(_:). Inserted characters inherit any attributes present at the insertion point.

## See Also

### Accessing Views into the Attributed String

var characters: AttributedString.CharacterView

The characters of the attributed string, as a view into the underlying string.

**Required**

var runs: AttributedString.Runs

The attributed runs of the attributed string, as a view into the underlying string.

**Required**

