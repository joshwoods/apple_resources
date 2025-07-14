

- Foundation
-  NSExistsCommand 

Class

# NSExistsCommand

A command that determines whether a scriptable object exists.

Mac Catalyst 13.0+macOS 10.0+

``` source
class NSExistsCommand
```

## Overview

An instance of `NSExistsCommand` determines whether a specified scriptable object, such as a word, paragraph, or image, exists.

When an instance of `NSExistsCommand` is executed, it evaluates the receiver specifier for the command to determine if it specifies any objects.

`NSExistsCommand` is part of Cocoa’s built-in scripting support. Most applications don’t need to subclass `NSExistsCommand`.

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

### Related Documentation

Cocoa Scripting Guide

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

class NSGetCommand

A command that retrieves a value or object from a scriptable object.

class NSCloneCommand

A command that clones one or more scriptable objects.

class NSCountCommand

A command that counts the number of objects of a specified class in the specified object container.

class NSCloseCommand

A command that closes one or more scriptable objects.

