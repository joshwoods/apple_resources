

- AppKit
- NSFormCell
-  placeholderString 

Instance Property

# placeholderString

The cell’s plain text placeholder string.

macOS

``` source
@MainActor
var placeholderString: String? { get set }
```

## Discussion

If this property returns `nil`, you can also call `placeholderAttributedString` to see if the cell has an attributed placeholder string. Note that invoking this method clears out any attributed string set by the placeholderAttributedString property.

## See Also

### Asking About Placeholder Values

var placeholderAttributedString: NSAttributedString?

The cell’s attributed placeholder string.

