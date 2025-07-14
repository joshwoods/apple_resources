

- AppKit
- NSAccessibilityContainsTransientUI
-  accessibilityPerformShowAlternateUI() 

Instance Method

# accessibilityPerformShowAlternateUI()

Displays the accessibility element’s alternative UI.

macOS

``` source
func accessibilityPerformShowAlternateUI() -> Bool
```

**Required**

## Return Value

true if the action was successfully triggered; otherwise, false. This method does not indicate the success or failure of the action, just the fact that the action was successfully triggered.

## Discussion

Use this method to trigger changes to the UI due to a mouse-hover or similar event.

## See Also

### Supporting Accessibility

func accessibilityPerformShowDefaultUI() -> Bool

Returns to the accessibility element’s original UI.

**Required**

func isAccessibilityAlternateUIVisible() -> Bool

Returns a Boolean value that determines whether the accessibility element’s alternative UI is currently visible.

**Required**

