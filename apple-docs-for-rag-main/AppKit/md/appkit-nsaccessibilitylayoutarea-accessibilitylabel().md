

- AppKit
- NSAccessibilityLayoutArea
-  accessibilityLabel() 

Instance Method

# accessibilityLabel()

Returns a short description of the layout area.

macOS

``` source
func accessibilityLabel() -> String
```

**Required**

## Return Value

The description of the layout area.

## Discussion

This method is the getter for the NSAccessibilityProtocol protocol’s accessibilityLabel property.

Do not include the control’s type in the label (for example, use `Canvas`, not `Canvas Layout Area`). If possible use a single word. To help ensure that accessibility clients such as VoiceOver read the label with the correct intonation, start this label with a capital letter. Do not put a period at the end. Always localize the label.

## See Also

### Supporting Accessibility

func accessibilityChildren() -> [Any]?

Returns the accessibility element’s children in the accessibility hierarchy.

**Required**

var accessibilityFocusedUIElement: Any

The child accessibility element with the current focus.

**Required**

func accessibilitySelectedChildren() -> [Any]?

Returns the layout area’s currently selected children.

**Required**

