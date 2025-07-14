

- AppKit
- NSAccessibilityContainsTransientUI
-  accessibilityPerformShowDefaultUI() 

Instance Method

# accessibilityPerformShowDefaultUI()

Returns to the accessibility element’s original UI.

macOS

``` source
func accessibilityPerformShowDefaultUI() -> Bool
```

**Required**

## Return Value

true if the action was successfully triggered; otherwise, false. This method does not indicate the success or failure of the action, just the fact that the action was successfully triggered.

## Discussion

Call this method after successfully calling accessibilityPerformShowAlternateUI() to return to the original UI.

## See Also

### Supporting Accessibility

func accessibilityPerformShowAlternateUI() -> Bool

Displays the accessibility element’s alternative UI.

**Required**

func isAccessibilityAlternateUIVisible() -> Bool

Returns a Boolean value that determines whether the accessibility element’s alternative UI is currently visible.

**Required**

