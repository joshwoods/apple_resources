

- UIKit
- UIBarButtonItem
-  primaryAction 

Instance Property

# primaryAction

The action associated with the item.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@NSCopying @MainActor
var primaryAction: UIAction? { get set }
```

## Discussion

When you assign a new value to this property, the title and image of the item update to match the primary action’s title and image.

If this property has a non-`nil` value, the system ignores the item’s target and action properties.

## See Also

### Managing the action

var changesSelectionAsPrimaryAction: Bool

A Boolean value that indicates whether the button represents an action or selection.

var action: Selector?

The selector defining the action message to send to the target object when the user taps this bar button item.

var target: AnyObject?

The object that receives an action when the user selects the item.

