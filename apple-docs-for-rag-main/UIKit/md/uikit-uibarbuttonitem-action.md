

- UIKit
- UIBarButtonItem
-  action 

Instance Property

# action

The selector defining the action message to send to the target object when the user taps this bar button item.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var action: Selector? { get set }
```

## Discussion

If the value of this property is `nil`, no action message is sent. The default value is `nil`.

## See Also

### Managing the action

var primaryAction: UIAction?

The action associated with the item.

var changesSelectionAsPrimaryAction: Bool

A Boolean value that indicates whether the button represents an action or selection.

var target: AnyObject?

The object that receives an action when the user selects the item.

