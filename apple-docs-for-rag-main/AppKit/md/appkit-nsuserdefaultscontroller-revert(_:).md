

- AppKit
- NSUserDefaultsController
-  revert(\_:) 

Instance Method

# revert(\_:)

Causes the receiver to discard any unsaved changes to bound user default properties, restoring their previous values.

macOS

``` source
@IBAction @MainActor
func revert(_ sender: Any?)
```

## Discussion

The receiver invokes discardEditing on any currently registered editors. The `sender` is typically the object that invoked this method.

If appliesImmediately is true, this method only causes any bound editors with uncommitted changes to discard their edits.

## See Also

### Managing user defaults values

var defaults: UserDefaults

Returns the instance of NSUserDefaults in use by the receiver.

var initialValues: [String : Any]?

Returns a dictionary containing the receiver’s initial default values.

var hasUnappliedChanges: Bool

Returns whether the receiver has user default values that have not been saved to NSUserDefaults.

var appliesImmediately: Bool

Returns whether any changes made to bound user default properties are saved immediately.

var values: Any

Returns a key value coding compliant object that is used to access the user default properties.

func revertToInitialValues(Any?)

Causes the receiver to discard all edits and replace the values of all the user default properties with any corresponding values in the initialValues dictionary.

func save(Any?)

Saves the values of the receiver’s user default properties.

