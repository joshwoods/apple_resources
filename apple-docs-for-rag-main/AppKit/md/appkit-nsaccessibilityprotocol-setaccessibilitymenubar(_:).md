

- AppKit
- NSAccessibilityProtocol
-  setAccessibilityMenuBar(\_:) 

Instance Method

# setAccessibilityMenuBar(\_:)

Sets the app’s menu bar.

macOS 10.10+

``` source
func setAccessibilityMenuBar(_ accessibilityMenuBar: Any?)
```

**Required**

## See Also

### Managing Apps

func accessibilityExtrasMenuBar() -> Any?

Returns the icon for the app’s menu bar extra.

**Required**

func setAccessibilityExtrasMenuBar(Any?)

Sets the icon for the app’s menu bar extra.

**Required**

func isAccessibilityFrontmost() -> Bool

Returns a Boolean value that determines whether the app is the frontmost app.

**Required**

func setAccessibilityFrontmost(Bool)

Sets a Boolean value that determines whether the app is the frontmost app.

**Required**

func isAccessibilityHidden() -> Bool

Returns a Boolean value that determines whether the app is in a hidden state.

**Required**

func setAccessibilityHidden(Bool)

Sets a Boolean value that determines whether the app is in a hidden state.

**Required**

func accessibilityMainWindow() -> Any?

Returns the app’s main window.

**Required**

func setAccessibilityMainWindow(Any?)

Sets the app’s main window.

**Required**

func accessibilityMenuBar() -> Any?

Returns the app’s menu bar.

**Required**

func accessibilityWindows() -> [Any]?

Returns an array that contains all the app’s windows.

**Required**

func setAccessibilityWindows([Any]?)

Sets the array that contains all the app’s windows.

**Required**

