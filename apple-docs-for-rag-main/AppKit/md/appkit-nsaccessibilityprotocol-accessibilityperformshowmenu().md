

- AppKit
- NSAccessibilityProtocol
-  accessibilityPerformShowMenu() 

Instance Method

# accessibilityPerformShowMenu()

Displays the menu accessibility element.

macOS 10.10+

``` source
func accessibilityPerformShowMenu() -> Bool
```

**Required**

## Return Value

true if the action was successfully triggered; otherwise, false. This method does not indicate the success or failure of the action, just the fact that the action was successfully triggered.

## Discussion

Use this method to display the contextual menu for the element.

## See Also

### Showing User Interface Elements

func accessibilityPerformShowAlternateUI() -> Bool

Displays the accessibility element’s alternative UI.

**Required**

func accessibilityPerformShowDefaultUI() -> Bool

Returns to the accessibility element’s original UI.

**Required**

func accessibilityPerformRaise() -> Bool

Brings the window to the front.

**Required**

