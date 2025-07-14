

- AppKit
- NSFormCell
-  placeholderAttributedString 

Instance Property

# placeholderAttributedString

The cell’s attributed placeholder string.

macOS

``` source
@NSCopying @MainActor
var placeholderAttributedString: NSAttributedString? { get set }
```

## Discussion

If this property returns `nil`, you can also call `placeholderString` to see if the cell has a plain text placeholder string.

## See Also

### Asking About Placeholder Values

var placeholderString: String?

The cell’s plain text placeholder string.

