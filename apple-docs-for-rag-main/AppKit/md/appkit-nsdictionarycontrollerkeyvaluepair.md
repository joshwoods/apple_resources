

- AppKit
-  NSDictionaryControllerKeyValuePair 

Class

# NSDictionaryControllerKeyValuePair

A set of methods implemented by arranged objects to give access to information about those objects.

macOS 10.11+

``` source
class NSDictionaryControllerKeyValuePair
```

## Overview

NSDictionaryControllerKeyValuePair is an informal protocol that is implemented by objects returned by the NSDictionaryController method arrangedObjects. See NSDictionaryController for more information.

## Topics

### Instance Properties

var isExplicitlyIncluded: Bool

var key: String?

var localizedKey: String?

var value: Any?

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Key-Value Data

class NSDictionaryController

A bindings-compatible controller that manages the display and editing of a dictionary of key-value pairs.

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

