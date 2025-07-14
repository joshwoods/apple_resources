

- AppKit
- NSUserDefaultsController
-  defaults 

Instance Property

# defaults

Returns the instance of NSUserDefaults in use by the receiver.

macOS

``` source
var defaults: UserDefaults { get }
```

## Discussion

This property is observable using key-value observing.

## See Also

### Managing user defaults values

var initialValues: [String : Any]?

Returns a dictionary containing the receiver’s initial default values.

var hasUnappliedChanges: Bool

Returns whether the receiver has user default values that have not been saved to NSUserDefaults.

var appliesImmediately: Bool

Returns whether any changes made to bound user default properties are saved immediately.

var values: Any

Returns a key value coding compliant object that is used to access the user default properties.

func revert(Any?)

Causes the receiver to discard any unsaved changes to bound user default properties, restoring their previous values.

func revertToInitialValues(Any?)

Causes the receiver to discard all edits and replace the values of all the user default properties with any corresponding values in the initialValues dictionary.

func save(Any?)

Saves the values of the receiver’s user default properties.

