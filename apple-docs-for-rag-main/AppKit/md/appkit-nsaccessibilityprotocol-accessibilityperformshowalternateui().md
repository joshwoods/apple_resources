

- AppKit
- NSAccessibilityProtocol
-  accessibilityPerformShowAlternateUI() 

Instance Method

# accessibilityPerformShowAlternateUI()

Displays the accessibility element’s alternative UI.

macOS 10.10+

``` source
func accessibilityPerformShowAlternateUI() -> Bool
```

**Required**

## Return Value

true if the action was successfully triggered; otherwise, false. This method does not indicate the success or failure of the action, just the fact that the action was successfully triggered.

## Discussion

Use this method to trigger changes to the UI due to a mouse-hover or similar event.

## See Also

### Showing User Interface Elements

func accessibilityPerformShowDefaultUI() -> Bool

Returns to the accessibility element’s original UI.

**Required**

func accessibilityPerformShowMenu() -> Bool

Displays the menu accessibility element.

**Required**

func accessibilityPerformRaise() -> Bool

Brings the window to the front.

**Required**

