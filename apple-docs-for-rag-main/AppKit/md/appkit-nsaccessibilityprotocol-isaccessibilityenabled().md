

- AppKit
- NSAccessibilityProtocol
-  isAccessibilityEnabled() 

Instance Method

# isAccessibilityEnabled()

Returns a Boolean value that determines whether the accessibility element responds to user events.

macOS 10.10+

``` source
func isAccessibilityEnabled() -> Bool
```

**Required**

## See Also

### Configuring Accessibility

func isAccessibilityElement() -> Bool

Returns a Boolean value that determines whether the accessibility element participates in the accessibility hierarchy.

**Required**

func setAccessibilityElement(Bool)

Sets a Boolean value that determines whether the accessibility element participates in the accessibility hierarchy.

**Required**

func setAccessibilityEnabled(Bool)

Sets a Boolean value that determines whether the accessibility element responds to user events.

**Required**

func accessibilityFrame() -> NSRect

Returns the accessibility element’s frame in screen coordinates.

**Required**

func setAccessibilityFrame(NSRect)

Sets the accessibility element’s frame in screen coordinates.

**Required**

func accessibilityHelp() -> String?

Returns the help text for the accessibility element.

**Required**

func setAccessibilityHelp(String?)

Sets the help text for the accessibility element.

**Required**

func accessibilityLabel() -> String?

Returns a short description of the accessibility element.

**Required**

func setAccessibilityLabel(String?)

Sets a short description of the accessibility element.

**Required**

func accessibilityTitle() -> String?

Returns the title of the accessibility element—for example, a button’s visible text.

**Required**

func setAccessibilityTitle(String?)

Sets the title of the accessibility element.

**Required**

func accessibilityValue() -> Any?

Returns the accessibility element’s value.

**Required**

func setAccessibilityValue(Any?)

Sets the accessibility element’s value.

**Required**

func isAccessibilitySelectorAllowed(Selector) -> Bool

Returns a Boolean value that indicates whether assistive apps can invoke the specified selector on the accessibility element.

**Required**

