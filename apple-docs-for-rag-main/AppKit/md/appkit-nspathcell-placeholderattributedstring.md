

- AppKit
- NSPathCell
-  placeholderAttributedString 

Instance Property

# placeholderAttributedString

Sets the value of the placeholder attributed string.

macOS 10.5+

``` source
@NSCopying @MainActor
var placeholderAttributedString: NSAttributedString? { get set }
```

## Parameters 

`string`  

The string to set for the placeholder attributed string.

## Discussion

If the `NSPathCell` object contains no `NSPathComponentCell` objects, the placeholder attributed string is drawn in their place, if it is not `nil`. If the placeholder attributed string is `nil`, the (non-attributed) placeholder string is drawn with default attributes, if it is not `nil`.

## See Also

### Setting Cell Appearance

var placeholderString: String?

Returns the placeholder string.

var backgroundColor: NSColor?

Returns the current background color of the receiver.

