

- AppKit
-  NSDictionaryController 

Class

# NSDictionaryController

A bindings-compatible controller that manages the display and editing of a dictionary of key-value pairs.

macOS 10.5+

``` source
class NSDictionaryController
```

## Overview

NSDictionaryController transforms the contents of a dictionary into an array of key-value pairs that can be bound to user interface items such as the columns of an NSTableView.

The content of an NSDictionaryController instance is specified using the inherited method content or by binding an NSDictionary instance to the contentDictionary binding. New key/value pairs inserted into the dictionary are created using the newObject() method. The initial key name is set to the string returned by initialKey . The initial key name is copied to the newly inserted object, while the object returned by initialValue is simply retained. As new items are inserted the controller enumerates the initial key name, resulting in key names such as “key”, “key1”, “key2”, and so on. This behavior can be customized by overriding newObject().

An NSDictionaryController instance can be configured to exclude specified keys in a dictionary from being returned by arrangedObjects using the excludedKeys property. Similarly, you can specify an array of key names that are always included in the arranged objects, even if they are not present in the content dictionary, using the includedKeys property.

NSDictionaryController supports providing localized key names for the keys in the dictionary, allowing a user-friendly representation of the key name to be displayed. The localized key names are specified by a dictionary (using localizedKeyDictionary) or by providing a strings table (using localizedKeyDictionary).

The arrangedObjects method returns an array of objects that implement the NSDictionaryControllerKeyValuePair informal protocol. User interface controls are bound to the arranged objects array using key paths such as: `arrangedObjects.key` (displays the key name), `arrangedObjects.value` (displays the value for the key), or `arrangedObjects.localizedKey` (displays the localized key name). See NSDictionaryControllerKeyValuePair for more information.

Note

You must enable the “Validates Immediately” option for the value binding of all controls that edit the key names or values returned by arrangedObjects.

NSDictionaryController overrides arrangedObjects to return an array of objects that implement the NSDictionaryControllerKeyValuePair informal protocol. See NSDictionaryControllerKeyValuePair and Cocoa Bindings Programming Topics for more information.

The constants listed below are used to specify a binding to bind(_:to:withKeyPath:options:), infoForBinding(_:), unbind(_:), and valueClassForBinding(_:). See the Cocoa Bindings Reference for more information.

- contentDictionary

- includedKeys

- excludedKeys

- localizedKeyDictionary

- initialKey

- initialValue

## Topics

### Arranging Objects

var arrangedObjects: Any

An array containing the receiver’s content objects arranged using arrange(_:).

### Creating New Entries

func newObject() -> NSDictionaryControllerKeyValuePair

Creates and returns a new key-value pair to represent an entry in the content dictionary.

### Localizing Key Names

var localizedKeyDictionary: [String : String]

The localized key names that are displayed by the receiver in place of the key names.

var localizedKeyTable: String?

the strings file used to localize key names.

### Keys to Display

var includedKeys: [String]

The key names that are represented by a key-value pair, even if they are not present in the receiver’s content dictionary.

var excludedKeys: [String]

The key names that are never displayed in the user interface items bound to the receiver.

### Setting Initial Key and Values

var initialKey: String

The string used as the initial key name for a newly inserted item.

var initialValue: Any

The string used as the initial value for a newly inserted item.

## Relationships

### Inherits From

- NSArrayController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSEditor
- NSEditorRegistration
- NSObjectProtocol

## See Also

### Key-Value Data

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

Binding dictionary keys

These constants define keys in the binding information dictionary.

