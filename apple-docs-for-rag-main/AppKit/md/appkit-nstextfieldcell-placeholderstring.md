

- AppKit
- NSTextFieldCell
-  placeholderString 

Instance Property

# placeholderString

The placeholder text for the cell, specified as a plain text string.

macOS

``` source
@MainActor
var placeholderString: String? { get set }
```

## Discussion

Assigning a new value to this property also clears out any value set for the placeholderAttributedString property.

## See Also

### Managing Placeholder Strings

var placeholderAttributedString: NSAttributedString?

The placeholder text for the cell, specified as an attributed string.

