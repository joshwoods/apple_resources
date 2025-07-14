

- AppKit
- NSAccessibilityProtocol
-  accessibilityDecrementButton() 

Instance Method

# accessibilityDecrementButton()

Returns the decrement button for the stepper accessibility element.

macOS 10.10+

``` source
func accessibilityDecrementButton() -> Any?
```

**Required**

## See Also

### Incrementing, Decrementing, and Deleting Values

func accessibilityIncrementButton() -> Any?

Returns the increment button for the stepper accessibility element.

**Required**

func setAccessibilityIncrementButton(Any?)

Sets the increment button for the stepper accessibility element.

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

