

- AppKit
- NSAccessibilityContainsTransientUI
-  isAccessibilityAlternateUIVisible() 

Instance Method

# isAccessibilityAlternateUIVisible()

Returns a Boolean value that determines whether the accessibility element’s alternative UI is currently visible.

macOS

``` source
func isAccessibilityAlternateUIVisible() -> Bool
```

**Required**

## Return Value

Use this property for elements that present an alternate UI—for example, when the pointer hovers over an interface element for a few seconds.

## See Also

### Supporting Accessibility

func accessibilityPerformShowAlternateUI() -> Bool

Displays the accessibility element’s alternative UI.

**Required**

func accessibilityPerformShowDefaultUI() -> Bool

Returns to the accessibility element’s original UI.

**Required**

