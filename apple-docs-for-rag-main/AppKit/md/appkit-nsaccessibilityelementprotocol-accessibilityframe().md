

- AppKit
- NSAccessibilityElementProtocol
-  accessibilityFrame() 

Instance Method

# accessibilityFrame()

Returns the accessibility element’s frame in screen coordinates.

macOS

``` source
func accessibilityFrame() -> NSRect
```

**Required**

## Return Value

The element’s frame in screen coordinates.

## Discussion

This method is the getter for the NSAccessibilityProtocol protocol’s accessibilityFrame property. This method is called whenever accessibility clients request the size or position attributes.

Note

If you are working with an NSAccessibilityElement subclass, use the accessibilityFrameInParentSpace property instead. The accessibilityFrameInParentSpace property ensures that accessibility element objects move when their parents move.

## See Also

### Supporting Accessibility

func accessibilityIdentifier() -> String

Returns the accessibility element’s identity.

func accessibilityParent() -> Any?

Returns the accessibility element’s parent in the accessibility hierarchy.

**Required**

func isAccessibilityFocused() -> Bool

Returns a Boolean value that indicates whether the accessibility element has the keyboard focus.

