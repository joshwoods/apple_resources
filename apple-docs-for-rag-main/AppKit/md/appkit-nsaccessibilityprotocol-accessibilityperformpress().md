

- AppKit
- NSAccessibilityProtocol
-  accessibilityPerformPress() 

Instance Method

# accessibilityPerformPress()

Simulates clicking the accessibility element.

macOS 10.10+

``` source
func accessibilityPerformPress() -> Bool
```

**Required**

## Return Value

true if the action was successfully triggered; otherwise, false. This method does not indicate the success or failure of the action, just the fact that the action was successfully triggered.

## Discussion

Use this method on elements that behave like buttons.

## See Also

### Selecting Elements

func accessibilityPerformPick() -> Bool

Selects the accessibility element.

**Required**

