

- AppKit
-  NSAccessibilityCustomAction 

Class

# NSAccessibilityCustomAction

A custom action to perform on an accessible object.

macOS 10.13+

``` source
class NSAccessibilityCustomAction
```

## Overview

Apps that support custom actions can create instances of this class, specifying the user-readable name of the action, and either a handler closure or the object and selector to use when performing the action. Assistive apps display custom actions in response to specific user cues. For example, VoiceOver lets users access actions quickly using the Actions rotor.

After creating an instance of this class, add it to the accessibilityCustomActions property of an appropriate accessible object.

## Topics

### Creating a Custom Action

init(name: String, handler: (() -> Bool)?)

Creates a custom action object with the specified name and handler.

init(name: String, target: any NSObjectProtocol, selector: Selector)

Creates a custom action object with the specified name, target, and selector.

### Getting the Action Name

var name: String

A localized name that describes the action.

### Getting the Action

var handler: (() -> Bool)?

The closure that handles the execution of the action.

var target: (any NSObjectProtocol)?

The object that performs the action through a selector.

var selector: Selector?

The method to call on the target to perform the action.

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

### Assigning Actions

func accessibilityCustomActions() -> [NSAccessibilityCustomAction]?

Returns the custom actions of the current accessibility element.

**Required**

func setAccessibilityCustomActions([NSAccessibilityCustomAction]?)

Sets the custom actions of the current accessibility element.

**Required**

