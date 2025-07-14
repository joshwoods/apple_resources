

- AppKit
- NSAccessibilityElementProtocol
-  accessibilityIdentifier() 

Instance Method

# accessibilityIdentifier()

Returns the accessibility element’s identity.

macOS

``` source
optional func accessibilityIdentifier() -> String
```

## Return Value

Returns the unique ID for the accessibility element. It is often used in automated testing.

## Discussion

This method is the getter for the NSAccessibilityProtocol protocol’s accessibilityIdentifier property.

## See Also

### Supporting Accessibility

func accessibilityFrame() -> NSRect

Returns the accessibility element’s frame in screen coordinates.

**Required**

func accessibilityParent() -> Any?

Returns the accessibility element’s parent in the accessibility hierarchy.

**Required**

func isAccessibilityFocused() -> Bool

Returns a Boolean value that indicates whether the accessibility element has the keyboard focus.

