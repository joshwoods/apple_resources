

- AppKit
- NSAccessibilityElementProtocol
-  accessibilityParent() 

Instance Method

# accessibilityParent()

Returns the accessibility element’s parent in the accessibility hierarchy.

macOS

``` source
func accessibilityParent() -> Any?
```

**Required**

## Return Value

The element’s parent in the accessibility hierarchy.

## Discussion

This method is the getter for the NSAccessibilityProtocol protocol’s accessibilityParent property.

## See Also

### Supporting Accessibility

func accessibilityFrame() -> NSRect

Returns the accessibility element’s frame in screen coordinates.

**Required**

func accessibilityIdentifier() -> String

Returns the accessibility element’s identity.

func isAccessibilityFocused() -> Bool

Returns a Boolean value that indicates whether the accessibility element has the keyboard focus.

