

- UIKit
- UIBarButtonItem
-  target 

Instance Property

# target

The object that receives an action when the user selects the item.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
weak var target: AnyObject? { get set }
```

## Discussion

If `nil`, the action message is passed up the responder chain where it may be handled by any object implementing a method corresponding to the selector held by the action property. The default value is `nil`.

## See Also

### Managing the action

var primaryAction: UIAction?

The action associated with the item.

var changesSelectionAsPrimaryAction: Bool

A Boolean value that indicates whether the button represents an action or selection.

var action: Selector?

The selector defining the action message to send to the target object when the user taps this bar button item.

