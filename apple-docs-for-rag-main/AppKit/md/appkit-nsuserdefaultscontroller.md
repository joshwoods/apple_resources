

- AppKit
-  NSUserDefaultsController 

Class

# NSUserDefaultsController

A controller that accesses user preference information for your app from the user’s defaults database.

macOS

``` source
class NSUserDefaultsController
```

## Overview

NSUserDefaultsController is a Cocoa bindings–compatible controller class. Properties of the shared instance of this class can be bound to user interface elements to access and modify values stored in UserDefaults.

## Topics

### Obtaining the shared instance

class var shared: NSUserDefaultsController

Returns the shared instance of NSUserDefaultsController, creating it if necessary.

### Initializing a user defaults controller

init(defaults: UserDefaults?, initialValues: [String : Any]?)

Returns an initialized NSUserDefaultsController object using the NSUserDefaults instance specified in `defaults` and the initial default values contained in the `initialValues` dictionary.

init?(coder: NSCoder)

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

func revert(Any?)

Causes the receiver to discard any unsaved changes to bound user default properties, restoring their previous values.

func revertToInitialValues(Any?)

Causes the receiver to discard all edits and replace the values of all the user default properties with any corresponding values in the initialValues dictionary.

func save(Any?)

Saves the values of the receiver’s user default properties.

## Relationships

### Inherits From

- NSController

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

### User Preferences

class NSUbiquitousKeyValueStore

An iCloud-based container of key-value pairs you use to share data among instances of your app running on a user's connected devices.

