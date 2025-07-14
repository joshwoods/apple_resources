

- Foundation
-  NSCloseCommand 

Class

# NSCloseCommand

A command that closes one or more scriptable objects.

Mac Catalyst 13.0+macOS 10.0+

``` source
class NSCloseCommand
```

## Overview

An instance of `NSCloseCommand` closes the specified scriptable object or objects—typically a document or window (and its associated document, if any). The command may optionally specify a location to save in and how to handle modified documents (by automatically saving changes, not saving them, or asking the user).

`NSCloseCommand` is part of Cocoa’s built-in scripting support. It works automatically to support the `close` command through key-value coding. Most applications don’t need to subclass `NSCloseCommand` or call its methods.

## Topics

### Accessing save options

var saveOptions: NSSaveOptions

Returns a constant indicating how to deal with closing any modified documents.

### Constants

enum NSSaveOptions

The saveOptions method returns one of the following constants to indicate how to deal with saving any modified documents:

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

class NSCloneCommand

A command that clones one or more scriptable objects.

class NSCountCommand

A command that counts the number of objects of a specified class in the specified object container.

