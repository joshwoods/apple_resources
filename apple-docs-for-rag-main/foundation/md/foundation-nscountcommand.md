

- Foundation
-  NSCountCommand 

Class

# NSCountCommand

A command that counts the number of objects of a specified class in the specified object container.

Mac Catalyst 13.0+macOS 10.0+

``` source
class NSCountCommand
```

## Overview

An instance of `NSCountCommand` counts the number of objects of a specified class in the specified object container (such as the number of words in a paragraph or document) and returns the result.

`NSCountCommand` is part of Cocoa’s built-in scripting support. It works automatically to support the `count` command through key-value coding. Most applications don’t need to subclass `NSCountCommand` or call its methods.

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

class NSExistsCommand

A command that determines whether a scriptable object exists.

class NSGetCommand

A command that retrieves a value or object from a scriptable object.

class NSCloneCommand

A command that clones one or more scriptable objects.

class NSCloseCommand

A command that closes one or more scriptable objects.

