

- AppKit
- NSAccessibilityProtocol
-  accessibilityPerformRaise() 

Instance Method

# accessibilityPerformRaise()

Brings the window to the front.

macOS 10.10+

``` source
func accessibilityPerformRaise() -> Bool
```

**Required**

## Return Value

true if the action was successfully triggered; otherwise, false. This method does not indicate the success or failure of the action, just the fact that the action was successfully triggered.

## Discussion

The window behaves as if you had clicked on the window’s title bar.

## See Also

### Showing User Interface Elements

func accessibilityPerformShowAlternateUI() -> Bool

Displays the accessibility element’s alternative UI.

**Required**

func accessibilityPerformShowDefaultUI() -> Bool

Returns to the accessibility element’s original UI.

**Required**

func accessibilityPerformShowMenu() -> Bool

Displays the menu accessibility element.

**Required**

