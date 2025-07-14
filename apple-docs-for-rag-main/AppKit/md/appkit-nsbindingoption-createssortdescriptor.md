

- AppKit
- NSBindingOption
-  createsSortDescriptor 

Type Property

# createsSortDescriptor

An `NSNumber` object containing a Boolean value that determines if a sort descriptor is created for a table column.

macOS

``` source
static let createsSortDescriptor: NSBindingOption
```

## Discussion

If this value is false, then the table column does not allow sorting.

## See Also

### Binding Options

static let allowsEditingMultipleValuesSelection: NSBindingOption

An `NSNumber` object containing a Boolean value that determines if the binding allows editing when the value represents a multiple selection.

static let allowsNullArgument: NSBindingOption

An `NSNumber` object containing a Boolean value that determines if the argument bindings allows passing argument values of `nil`.

static let alwaysPresentsApplicationModalAlerts: NSBindingOption

A number containing a Boolean value that determines if validation and error alert panels displayed as a result of this binding are displayed as application modal alerts.

static let conditionallySetsEditable: NSBindingOption

An `NSNumber` object containing a Boolean value that determines if the editable state of the user interface item is automatically configured based on the controller’s selection.

static let conditionallySetsEnabled: NSBindingOption

An `NSNumber` object containing a Boolean value that determines if the enabled state of the user interface item is automatically configured based on the controller’s selection.

static let conditionallySetsHidden: NSBindingOption

An `NSNumber` object containing a Boolean value that determines if the hidden state of the user interface item is automatically configured based on the controller’s selection.

static let contentPlacementTag: NSBindingOption

A number that specifies the tag id of the popup menu item to replace with the content of the array.

static let continuouslyUpdatesValue: NSBindingOption

An `NSNumber` object containing a Boolean value that determines whether the value of the binding is updated as edits are made to the user interface item or is updated only when the user interface item resigns as the responder.

static let deletesObjectsOnRemove: NSBindingOption

An `NSNumber` object containing a Boolean value that determines if an object is deleted from the managed context immediately upon being removed from a relationship.

static let displayName: NSBindingOption

An `NSString` object containing a human readable string to be displayed for a predicate.

static let displayPattern: NSBindingOption

An `NSString` object that specifies a format string used to construct the final value of a string.

static let handlesContentAsCompoundValue: NSBindingOption

An `NSNumber` object containing a Boolean value that determines if the content is treated as a compound value.

static let insertsNullPlaceholder: NSBindingOption

An `NSNumber` object containing a Boolean value that determines if an additional item which represents `nil` is inserted into a matrix or pop-up menu before the items in the content array.

static let invokesSeparatelyWithArrayObjects: NSBindingOption

An `NSNumber` object containing a Boolean value that determines whether the specified selector is invoked with the array as the argument or is invoked repeatedly with each array item as an argument.

static let multipleValuesPlaceholder: NSBindingOption

An object that is used as a placeholder when the key path of the bound controller returns the `NSMultipleValuesMarker` marker for a binding.

