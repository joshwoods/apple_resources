

- AppKit
- NSTextField
-  isSelectable 

Instance Property

# isSelectable

A Boolean value that determines whether the user can select the content of the text field.

macOS

``` source
@MainActor
var isSelectable: Bool { get set }
```

## Discussion

If true, the text field becomes selectable but not editable. Use isEditable to make the text field selectable and editable. If false, the text is neither editable nor selectable.

## See Also

### Controlling Selection and Editing

var isEditable: Bool

A Boolean value that controls whether the user can edit the value in the text field.

