

- AppKit
- NSAccessibilityProtocol
-  accessibilityPerformCancel() 

Instance Method

# accessibilityPerformCancel()

Cancels the current operation.

macOS 10.10+

``` source
func accessibilityPerformCancel() -> Bool
```

**Required**

## Return Value

true if the action was successfully triggered; otherwise, false. This method does not indicate the success or failure of the action, just the fact that the action was successfully triggered.

## See Also

### Confirming and Canceling Operations

func accessibilityPerformConfirm() -> Bool

Simulates pressing Return in the accessibility element.

**Required**

