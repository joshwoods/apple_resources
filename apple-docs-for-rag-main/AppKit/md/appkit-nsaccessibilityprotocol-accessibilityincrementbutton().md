

- AppKit
- NSAccessibilityProtocol
-  accessibilityIncrementButton() 

Instance Method

# accessibilityIncrementButton()

Returns the increment button for the stepper accessibility element.

macOS 10.10+

``` source
func accessibilityIncrementButton() -> Any?
```

**Required**

## See Also

### Incrementing, Decrementing, and Deleting Values

func setAccessibilityIncrementButton(Any?)

Sets the increment button for the stepper accessibility element.

**Required**

func accessibilityDecrementButton() -> Any?

Returns the decrement button for the stepper accessibility element.

**Required**

func setAccessibilityDecrementButton(Any?)

Sets the decrement button for the stepper accessibility element.

**Required**

func accessibilityPerformIncrement() -> Bool

Increments the accessibility element’s value.

**Required**

func accessibilityPerformDecrement() -> Bool

Decrements the accessibility element’s value.

**Required**

func accessibilityPerformDelete() -> Bool

Deletes the accessibility element’s value.

**Required**

