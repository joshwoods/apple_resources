

- AppKit
- NSAccessibilityProtocol
-  accessibilityPerformIncrement() 

Instance Method

# accessibilityPerformIncrement()

Increments the accessibility element’s value.

macOS 10.10+

``` source
func accessibilityPerformIncrement() -> Bool
```

**Required**

## Return Value

true if the action was successfully triggered; otherwise, false. This method does not indicate the success or failure of the action, just the fact that the action was successfully triggered.

## Discussion

Use this method on elements that have an adjustable accessibilityValue property.

## See Also

### Incrementing, Decrementing, and Deleting Values

func accessibilityIncrementButton() -> Any?

Returns the increment button for the stepper accessibility element.

**Required**

func setAccessibilityIncrementButton(Any?)

Sets the increment button for the stepper accessibility element.

**Required**

func accessibilityDecrementButton() -> Any?

Returns the decrement button for the stepper accessibility element.

**Required**

func setAccessibilityDecrementButton(Any?)

Sets the decrement button for the stepper accessibility element.

**Required**

func accessibilityPerformDecrement() -> Bool

Decrements the accessibility element’s value.

**Required**

func accessibilityPerformDelete() -> Bool

Deletes the accessibility element’s value.

**Required**

