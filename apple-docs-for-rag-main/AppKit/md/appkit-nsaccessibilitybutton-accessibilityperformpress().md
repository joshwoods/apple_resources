

- AppKit
- NSAccessibilityButton
-  accessibilityPerformPress() 

Instance Method

# accessibilityPerformPress()

Simulates clicking the button.

macOS

``` source
func accessibilityPerformPress() -> Bool
```

**Required**

## Return Value

true if the action was successfully triggered; otherwise, false. This method does not indicate the success or failure of the action, just the fact that the action was successfully triggered.

## See Also

### Supporting Accessibility

func accessibilityLabel() -> String?

Returns a short description of the button.

**Required**

