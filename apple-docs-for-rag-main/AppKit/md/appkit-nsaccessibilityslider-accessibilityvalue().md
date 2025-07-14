

- AppKit
- NSAccessibilitySlider
-  accessibilityValue() 

Instance Method

# accessibilityValue()

Returns the slider’s value.

macOS

``` source
func accessibilityValue() -> Any?
```

**Required**

## Return Value

The value for the slider.

## Discussion

This method is the getter for the NSAccessibilityProtocol protocol’s accessibilityValue property.

## See Also

### Supporting Accessibility

func accessibilityLabel() -> String?

Returns a short description of the slider.

**Required**

func accessibilityPerformDecrement() -> Bool

Decrements the slider’s value.

**Required**

func accessibilityPerformIncrement() -> Bool

Increments the slider’s value.

**Required**

