

- Foundation
-  NSCreateCommand 

Class

# NSCreateCommand

A command that creates a scriptable object.

Mac Catalyst 13.0+macOS 10.0+

``` source
class NSCreateCommand
```

## Overview

An instance of `NSCreateCommand` creates the specified scriptable object (such as a document), optionally supplying the new object with the specified attributes. This command corresponds to AppleScript’s `make` command.

`NSCreateCommand` is part of Cocoa’s built-in scripting support. Most applications don’t need to subclass `NSCreateCommand` or invoke its methods.

When an instance of `NSCreateCommand` is executed, it creates a new object using `[[theClassToBeCreated allocWithZone:NULL] init]` (where `theClassToBeCreated` is the class of the object to be created), unless the command has a `with data` argument. In the latter case, the new object is created by invoking `[[NSScriptCoercionHandler sharedCoercionHandler] coerceValue:theDataAsAnObject toClass:theClassToBeCreated]`. Any properties specified by a `with properties` argument are then set in the new object using `-setScriptingProperties:`.

If an `NSCreateCommand` object with no argument corresponding to the `at` parameter is executed (for example, `tell application "Mail" to make new mailbox with properties {name:"testFolder"}`), and the receiver of the command (not necessarily the application object) has a to-many relationship to objects of the class to be instantiated, and the class description for the receiving class returns false when sent an `isLocationRequiredToCreateForKey:` message, the `NSCreateCommand` object creates a new object and sends the receiver an insertValue(_:at:inPropertyWithKey:) message to place the new object in the container. This is part of Cocoa’s scripting support for inserting newly-created objects into containers without explicitly specifying a location.

## Topics

### Getting information about a create command

var createClassDescription: NSScriptClassDescription

Returns the class description for the class that is to be created.

var resolvedKeyDictionary: [String : Any]

Returns a dictionary that contains the properties that were specified in the `make` Apple event command that has been converted to this `NSCreateCommand` object.

## Relationships

### Inherits From

- NSScriptCommand

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol

## See Also

### Script Commands

class NSScriptCommand

A self-contained scripting statement.

class NSQuitCommand

A command that quits the specified app.

class NSSetCommand

A command that sets one or more attributes or relationships to one or more values.

class NSMoveCommand

A command that moves one or more scriptable objects.

class NSDeleteCommand

A command that deletes a scriptable object.

class NSExistsCommand

A command that determines whether a scriptable object exists.

class NSGetCommand

A command that retrieves a value or object from a scriptable object.

class NSCloneCommand

A command that clones one or more scriptable objects.

class NSCountCommand

A command that counts the number of objects of a specified class in the specified object container.

class NSCloseCommand

A command that closes one or more scriptable objects.

