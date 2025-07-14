

- AppKit
- NSAccessibilityProtocol
-  accessibilityPerformPick() 

Instance Method

# accessibilityPerformPick()

Selects the accessibility element.

macOS 10.10+

``` source
func accessibilityPerformPick() -> Bool
```

**Required**

## Return Value

true if the action was successfully triggered; otherwise, false. This method does not indicate the success or failure of the action, just the fact that the action was successfully triggered.

## Discussion

Use this method on selectable elements, such as a menu item.

## See Also

### Selecting Elements

func accessibilityPerformPress() -> Bool

Simulates clicking the accessibility element.

**Required**

