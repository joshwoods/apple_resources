

- UIKit
- UIBarButtonItem
-  changesSelectionAsPrimaryAction 

Instance Property

# changesSelectionAsPrimaryAction

A Boolean value that indicates whether the button represents an action or selection.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
var changesSelectionAsPrimaryAction: Bool { get set }
```

## Discussion

When a button has this property set to true, the button changes to a toggle button where tapping it changes it between selected and unselected.

## See Also

### Managing the action

var primaryAction: UIAction?

The action associated with the item.

var action: Selector?

The selector defining the action message to send to the target object when the user taps this bar button item.

var target: AnyObject?

The object that receives an action when the user selects the item.

