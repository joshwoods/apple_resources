

- AppKit
- NSAccessibilityStepper
-  accessibilityLabel() 

Instance Method

# accessibilityLabel()

Returns a short description of the stepper.

macOS

``` source
func accessibilityLabel() -> String?
```

**Required**

## Return Value

The description of the stepper.

## Discussion

This method is the getter for the NSAccessibilityProtocol protocol’s accessibilityLabel property.

Do not include the control’s type in the label (for example, use `Volume`, not `Volume stepper`). If possible use a single word. To help ensure that accessibility clients such as VoiceOver read the label with the correct intonation, start this label with a capital letter. Do not put a period at the end. Always localize the label.

## See Also

### Supporting Accessibility

func accessibilityPerformDecrement() -> Bool

Decrements the stepper’s value.

**Required**

func accessibilityPerformIncrement() -> Bool

Increments the stepper’s value.

**Required**

func accessibilityValue() -> Any?

Returns the stepper’s value.

