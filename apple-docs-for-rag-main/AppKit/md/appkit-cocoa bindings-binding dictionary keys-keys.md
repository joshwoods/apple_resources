

- AppKit
- Cocoa Bindings
-  Binding dictionary keys 

API Collection

# Binding dictionary keys

These constants define keys in the binding information dictionary.

## Topics

### Constants

static let observedObject: NSBindingInfoKey

The object that is the observable controller of the binding.

static let observedKeyPath: NSBindingInfoKey

An `NSString` object containing the key path of the binding.

static let options: NSBindingInfoKey

An `NSDictionary` object containing key value pairs as specified in the options dictionary when the binding was created.

## See Also

### Key-Value Data

class NSDictionaryController

A bindings-compatible controller that manages the display and editing of a dictionary of key-value pairs.

class NSDictionaryControllerKeyValuePair

A set of methods implemented by arranged objects to give access to information about those objects.

struct NSBindingName

Values that specify a binding for certain methods.

struct NSBindingOption

struct NSBindingInfoKey

func NSIsControllerMarker(Any?) -> Bool

Tests whether a given object is special marker object used for indicating the state of a selection in relation to a key.

NSKeyValueBindingCreation

A set of methods that you can use to create and remove bindings between view objects and controllers, or between controllers and model objects.

