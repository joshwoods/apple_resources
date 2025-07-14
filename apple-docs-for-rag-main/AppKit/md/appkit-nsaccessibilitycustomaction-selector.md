

- AppKit
- NSAccessibilityCustomAction
-  selector 

Instance Property

# selector

The method to call on the target to perform the action.

macOS 10.13+

``` source
var selector: Selector? { get set }
```

## See Also

### Getting the Action

var handler: (() -> Bool)?

The closure that handles the execution of the action.

var target: (any NSObjectProtocol)?

The object that performs the action through a selector.

