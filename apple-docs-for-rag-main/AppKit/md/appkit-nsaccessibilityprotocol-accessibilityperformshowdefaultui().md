

- AppKit
- NSAccessibilityProtocol
-  accessibilityPerformShowDefaultUI() 

Instance Method

# accessibilityPerformShowDefaultUI()

Returns to the accessibility element’s original UI.

macOS 10.10+

``` source
func accessibilityPerformShowDefaultUI() -> Bool
```

**Required**

## Return Value

true if the action was successfully triggered; otherwise, false. This method does not indicate the success or failure of the action, just the fact that the action was successfully triggered.

## Discussion

Call this method after successfully calling accessibilityPerformShowAlternateUI() to return to the original UI.

## See Also

### Showing User Interface Elements

func accessibilityPerformShowAlternateUI() -> Bool

Displays the accessibility element’s alternative UI.

**Required**

func accessibilityPerformShowMenu() -> Bool

Displays the menu accessibility element.

**Required**

func accessibilityPerformRaise() -> Bool

Brings the window to the front.

**Required**

