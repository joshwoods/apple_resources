

- AppKit
- NSAccessibilityProtocol
-  setAccessibilityApplicationFocusedUIElement(\_:) 

Instance Method

# setAccessibilityApplicationFocusedUIElement(\_:)

Sets the child accessibility element with the current focus.

macOS 10.10+

``` source
func setAccessibilityApplicationFocusedUIElement(_ accessibilityApplicationFocusedUIElement: Any?)
```

**Required**

## See Also

### Setting the Focus

func accessibilityApplicationFocusedUIElement() -> Any?

Returns the child accessibility element with the current focus.

**Required**

func isAccessibilityFocused() -> Bool

Returns a Boolean value that determines whether the accessibility element has the keyboard focus.

**Required**

func setAccessibilityFocused(Bool)

Sets a Boolean value that determines whether the accessibility element has the keyboard focus.

**Required**

func accessibilityFocusedWindow() -> Any?

Returns the child window with the current focus.

**Required**

func setAccessibilityFocusedWindow(Any?)

Sets the child window with the current focus.

**Required**

func accessibilitySharedFocusElements() -> [Any]?

Returns the array of elements that shares the keyboard focus with the accessibility element.

**Required**

func setAccessibilitySharedFocusElements([Any]?)

Sets the array of elements that shares the keyboard focus with the accessibility element.

**Required**

