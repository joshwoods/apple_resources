

- Foundation
- AttributedStringProtocol
-  characters 

Instance Property

# characters

The characters of the attributed string, as a view into the underlying string.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var characters: AttributedString.CharacterView { get }
```

**Required**

## Discussion

Use the `AttributedString/characters` view when you want to look for specific string content. You can then use the resulting ranges to set attributes for specific parts of the AttributedString or AttributedSubstring.

You can also use this property to mutate the attributed string, using RangeReplaceableCollection methods, such as `insert(_:at:)` and append(_:). Inserted characters inherit any attributes present at the insertion point.

## See Also

### Accessing Views into the Attributed String

var unicodeScalars: AttributedString.UnicodeScalarView

The Unicode scalars of the attributed string, as a view into the underlying string.

**Required**

var runs: AttributedString.Runs

The attributed runs of the attributed string, as a view into the underlying string.

**Required**

