

- Foundation
-  NSCloneCommand 

Class

# NSCloneCommand

A command that clones one or more scriptable objects.

Mac Catalyst 13.0+macOS 10.0+

``` source
class NSCloneCommand
```

## Overview

An instance of `NSCloneCommand` clones the specified scriptable object or objects (such as words, paragraphs, images, and so on) and inserts them in the specified location, or the default location if no location is specified. The cloned scriptable objects typically correspond to objects in the application, but aren’t required to. This command corresponds to AppleScript’s `duplicate` command.

`NSCloneCommand` is part of Cocoa’s built-in scripting support. It works automatically to support the `duplicate` command through key-value coding. Most applications don’t need to subclass `NSCloneCommand` or invoke its methods.

When an instance of `NSCloneCommand` is executed, it clones the specified objects by sending them copyWithZone: messages.

## Topics

### Working with specifiers

var keySpecifier: NSScriptObjectSpecifier

Returns a specifier for the object or objects to be cloned.

func setReceiversSpecifier(NSScriptObjectSpecifier?)

Sets the receiver’s object specifier;.

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

class NSCreateCommand

A command that creates a scriptable object.

class NSDeleteCommand

A command that deletes a scriptable object.

class NSExistsCommand

A command that determines whether a scriptable object exists.

class NSGetCommand

A command that retrieves a value or object from a scriptable object.

class NSCountCommand

A command that counts the number of objects of a specified class in the specified object container.

class NSCloseCommand

A command that closes one or more scriptable objects.

