

- AppKit
- NSAccessibilitySlider
-  accessibilityLabel() 

Instance Method

# accessibilityLabel()

Returns a short description of the slider.

macOS

``` source
func accessibilityLabel() -> String?
```

**Required**

## Return Value

The description of the slider.

## Discussion

This method is the getter for the NSAccessibilityProtocol protocol’s accessibilityLabel property.

Do not include the control’s type in the label (for example, use `Volume`, not `Volume slider`). If possible use a single word. To help ensure that accessibility clients such as VoiceOver read the label with the correct intonation, start this label with a capital letter. Do not put a period at the end. Always localize the label.

## See Also

### Supporting Accessibility

func accessibilityPerformDecrement() -> Bool

Decrements the slider’s value.

**Required**

func accessibilityPerformIncrement() -> Bool

Increments the slider’s value.

**Required**

func accessibilityValue() -> Any?

Returns the slider’s value.

**Required**

