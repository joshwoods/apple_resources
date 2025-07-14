

- AppKit
- NSAccessibilityCustomAction
-  handler 

Instance Property

# handler

The closure that handles the execution of the action.

macOS 10.13+

``` source
var handler: (() -> Bool)? { get set }
```

## See Also

### Getting the Action

var target: (any NSObjectProtocol)?

The object that performs the action through a selector.

var selector: Selector?

The method to call on the target to perform the action.

