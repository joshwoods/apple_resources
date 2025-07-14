

- AppKit
- NSPathCell
-  placeholderString 

Instance Property

# placeholderString

Returns the placeholder string.

macOS 10.5+

``` source
@MainActor
var placeholderString: String? { get set }
```

## Return Value

The placeholder string.

## Discussion

If the `NSPathCell` object contains no `NSPathComponentCell` objects, the placeholder attributed string is drawn in their place, if it is not `nil`. If the placeholder attributed string is `nil`, the (non-attributed) placeholder string is drawn with default attributes, if it is not `nil`.

## See Also

### Setting Cell Appearance

var placeholderAttributedString: NSAttributedString?

Sets the value of the placeholder attributed string.

var backgroundColor: NSColor?

Returns the current background color of the receiver.

