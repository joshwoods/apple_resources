

- AppKit
- NSAccessibilityProtocol
-  accessibilityPerformConfirm() 

Instance Method

# accessibilityPerformConfirm()

Simulates pressing Return in the accessibility element.

macOS 10.10+

``` source
func accessibilityPerformConfirm() -> Bool
```

**Required**

## Return Value

true if the action was successfully triggered; otherwise, false. This method does not indicate the success or failure of the action, just the fact that the action was successfully triggered.

## Discussion

Use this method on elements that take keyboard input, such as a text field.

## See Also

### Confirming and Canceling Operations

func accessibilityPerformCancel() -> Bool

Cancels the current operation.

**Required**

