

- Foundation
-  NSQuitCommand 

Class

# NSQuitCommand

A command that quits the specified app.

Mac Catalyst 13.0+macOS 10.0+

``` source
class NSQuitCommand
```

## Overview

The quit command may optionally specify how to handle modified documents (automatically save changes, don’t save them, or ask the user). For details, see the description for the `quit` command in “Apple Events Sent By the Mac OS” in How Cocoa Applications Handle Apple Events in Cocoa Scripting Guide.

`NSQuitCommand` is part of Cocoa’s built-in scripting support. Most applications don’t need to subclass `NSQuitCommand` or call its methods.

## Topics

### Accessing options

var saveOptions: NSSaveOptions

Returns a constant indicating how to deal with closing any modified documents.

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

class NSCloneCommand

A command that clones one or more scriptable objects.

class NSCountCommand

A command that counts the number of objects of a specified class in the specified object container.

class NSCloseCommand

A command that closes one or more scriptable objects.

