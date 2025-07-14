

- AppKit
- NSAccessibilityStepper
-  accessibilityValue() 

Instance Method

# accessibilityValue()

Returns the stepper’s value.

macOS

``` source
optional func accessibilityValue() -> Any?
```

## Return Value

The value for the stepper.

## Discussion

This method is the getter for the NSAccessibilityProtocol protocol’s accessibilityValue property.

## See Also

### Supporting Accessibility

func accessibilityLabel() -> String?

Returns a short description of the stepper.

**Required**

func accessibilityPerformDecrement() -> Bool

Decrements the stepper’s value.

**Required**

func accessibilityPerformIncrement() -> Bool

Increments the stepper’s value.

**Required**

