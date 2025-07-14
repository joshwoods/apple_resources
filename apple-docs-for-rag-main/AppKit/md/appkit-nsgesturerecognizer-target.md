

- AppKit
- NSGestureRecognizer
-  target 

Instance Property

# target

The object that implements the action method.

macOS 10.10+

``` source
@MainActor
weak var target: AnyObject? { get set }
```

## Discussion

The object in this property must implement the method specified by the action property.

## See Also

### Accessing the Target and Action

var action: Selector?

The action method to call when the gesture is recognized.

