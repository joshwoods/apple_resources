

- AppKit
- NSAccessibilityCustomAction
-  target 

Instance Property

# target

The object that performs the action through a selector.

macOS 10.13+

``` source
weak var target: (any NSObjectProtocol)? { get set }
```

## See Also

### Getting the Action

var handler: (() -> Bool)?

The closure that handles the execution of the action.

var selector: Selector?

The method to call on the target to perform the action.

