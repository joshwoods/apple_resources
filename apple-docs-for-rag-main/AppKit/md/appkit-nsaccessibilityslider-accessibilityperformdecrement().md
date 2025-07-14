

- AppKit
- NSAccessibilitySlider
-  accessibilityPerformDecrement() 

Instance Method

# accessibilityPerformDecrement()

Decrements the slider’s value.

macOS

``` source
func accessibilityPerformDecrement() -> Bool
```

**Required**

## Return Value

true if the action was successfully triggered; otherwise, false. This method does not indicate the success or failure of the action, just the fact that the action was successfully triggered.

## Discussion

This method must post an valueChanged notification after changing the slider’s value.

## See Also

### Supporting Accessibility

func accessibilityLabel() -> String?

Returns a short description of the slider.

**Required**

func accessibilityPerformIncrement() -> Bool

Increments the slider’s value.

**Required**

func accessibilityValue() -> Any?

Returns the slider’s value.

**Required**

