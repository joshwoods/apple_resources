

- AppKit
- NSAccessibilitySwitch
-  accessibilityPerformDecrement() 

Instance Method

# accessibilityPerformDecrement()

Decrements the switch’s value.

macOS

``` source
optional func accessibilityPerformDecrement() -> Bool
```

## Return Value

true if the action was successfully triggered; otherwise, false. This method does not indicate the success or failure of the action, just the fact that the action was successfully triggered.

## Discussion

This method must post an valueChanged notification after changing the switch’s value.

## See Also

### Supporting Accessibility

func accessibilityPerformIncrement() -> Bool

Increments the switch’s value.

func accessibilityValue() -> String?

Returns the switch’s value.

**Required**

