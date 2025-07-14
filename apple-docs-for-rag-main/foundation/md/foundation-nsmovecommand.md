

- Foundation
-  NSMoveCommand 

Class

# NSMoveCommand

A command that moves one or more scriptable objects.

Mac Catalyst 13.0+macOS 10.0+

``` source
class NSMoveCommand
```

## Overview

An instance of `NSMoveCommand` moves the specified scriptable object or objects; for example, it may move words to a new location in a document or a file to a new directory.

`NSMoveCommand` is part of Cocoa’s built-in scripting support. It works automatically to support the `move` AppleScript command through key-value coding. Most applications don’t need to subclass `NSMoveCommand` or invoke its methods. However, for circumstances where you might choose to subclass this command, see “Modifying a Standard Command” in Script Commands in Cocoa Scripting Guide.

When an instance of `NSMoveCommand` is executed, it does not make copies of moved objects. It removes objects from the source container or containers, then inserts them into the destination container.

## Topics

### Working with specifiers

var keySpecifier: NSScriptObjectSpecifier

Returns a specifier for the object or objects to be moved.

func setReceiversSpecifier(NSScriptObjectSpecifier?)

Sets the receiver’s object specifier.

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

class NSCreateCommand

A command that creates a scriptable object.

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

