

- Foundation
- AttributedStringProtocol
-  runs 

Instance Property

# runs

The attributed runs of the attributed string, as a view into the underlying string.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var runs: AttributedString.Runs { get }
```

**Required**

## Discussion

Runs begin and end when the attributes for the characters change. Use this property to iterate over the runs with `for`-`in` syntax.

## See Also

### Accessing Views into the Attributed String

var characters: AttributedString.CharacterView

The characters of the attributed string, as a view into the underlying string.

**Required**

var unicodeScalars: AttributedString.UnicodeScalarView

The Unicode scalars of the attributed string, as a view into the underlying string.

**Required**

