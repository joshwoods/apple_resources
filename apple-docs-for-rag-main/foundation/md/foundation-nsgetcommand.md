

- Foundation
-  NSGetCommand 

Class

# NSGetCommand

A command that retrieves a value or object from a scriptable object.

Mac Catalyst 13.0+macOS 10.0+

``` source
class NSGetCommand
```

## Overview

An instance of `NSGetCommand` gets the specified value or object from the specified scriptable object: for example, the words from a paragraph or the name of a document.

When an instance of `NSGetCommand` is executed, it evaluates the specified receivers, gathers the specified data, if any, and packages it in a return Apple event.

`NSGetCommand` is part of Cocoa’s built-in scripting support. It works automatically to support the `get` command through key-value coding. Most applications don’t need to subclass `NSGetCommand` or call its methods.

For information on working with `get` commands, see Getting and Setting Properties and Elements in Cocoa Scripting Guide.

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

class NSCloneCommand

A command that clones one or more scriptable objects.

class NSCountCommand

A command that counts the number of objects of a specified class in the specified object container.

class NSCloseCommand

A command that closes one or more scriptable objects.

