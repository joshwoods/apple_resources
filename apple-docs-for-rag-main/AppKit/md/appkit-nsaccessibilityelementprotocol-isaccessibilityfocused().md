

- AppKit
- NSAccessibilityElementProtocol
-  isAccessibilityFocused() 

Instance Method

# isAccessibilityFocused()

Returns a Boolean value that indicates whether the accessibility element has the keyboard focus.

macOS

``` source
optional func isAccessibilityFocused() -> Bool
```

## Return Value

true if this element has the keyboard focus; otherwise, false.

## Discussion

This method is the getter for the NSAccessibilityProtocol protocol’s accessibilityFocused property.

## See Also

### Supporting Accessibility

func accessibilityFrame() -> NSRect

Returns the accessibility element’s frame in screen coordinates.

**Required**

func accessibilityIdentifier() -> String

Returns the accessibility element’s identity.

func accessibilityParent() -> Any?

Returns the accessibility element’s parent in the accessibility hierarchy.

**Required**

