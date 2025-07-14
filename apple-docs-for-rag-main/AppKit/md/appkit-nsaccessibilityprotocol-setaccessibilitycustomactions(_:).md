

- AppKit
- NSAccessibilityProtocol
-  setAccessibilityCustomActions(\_:) 

Instance Method

# setAccessibilityCustomActions(\_:)

Sets the custom actions of the current accessibility element.

macOS 10.13+

``` source
func setAccessibilityCustomActions(_ accessibilityCustomActions: [NSAccessibilityCustomAction]?)
```

**Required**

## See Also

### Assigning Actions

func accessibilityCustomActions() -> [NSAccessibilityCustomAction]?

Returns the custom actions of the current accessibility element.

**Required**

class NSAccessibilityCustomAction

A custom action to perform on an accessible object.

