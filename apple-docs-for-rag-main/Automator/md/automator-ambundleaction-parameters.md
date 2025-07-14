

- Automator
- AMBundleAction
-  parameters 

Instance Property

# parameters

The action’s parameters.

Mac Catalyst 14.0+macOS 10.4+

``` source
var parameters: NSMutableDictionary? { get set }
```

## Discussion

The parameters of an action reflect the choices made and values entered in the action’s user interface. Keys in the parameters dictionary identify specific user-interface objects. If an action uses the Cocoa bindings mechanism, the parameters of an AMBundleAction object are automatically set.

## See Also

### Managing Action Properties

var bundle: Bundle

The action’s bundle object.

var hasView: Bool

A Boolean value that indicates whether the action has a view associated with it.

var view: NSView?

The action’s view object.

