

- AppKit
- NSTextFieldCell
-  placeholderAttributedString 

Instance Property

# placeholderAttributedString

The placeholder text for the cell, specified as an attributed string.

macOS

``` source
@NSCopying @MainActor
var placeholderAttributedString: NSAttributedString? { get set }
```

## Discussion

Assigning a new value to this property also clears out any value set for the placeholderString property.

## See Also

### Managing Placeholder Strings

var placeholderString: String?

The placeholder text for the cell, specified as a plain text string.

