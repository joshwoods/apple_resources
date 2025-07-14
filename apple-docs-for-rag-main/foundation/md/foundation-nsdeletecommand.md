

- Foundation
-  NSDeleteCommand 

Class

# NSDeleteCommand

A command that deletes a scriptable object.

Mac Catalyst 13.0+macOS 10.0+

``` source
class NSDeleteCommand
```

## Overview

An instance of `NSDeleteCommand` deletes the specified scriptable object or objects (such as words, paragraphs, and so on).

Suppose, for example, a user executes a script that sends the command `delete the third rectangle in the first document` to the Sketch sample application (located in `/Developer/Examples/AppKit`). Cocoa creates an `NSDeleteCommand` object to perform the operation. When the command is executed, it uses the key-value coding mechanism (by invoking `removeValueAtIndex:fromPropertyWithKey:`) to remove the specified object or objects from their container. See the description for removeValue(at:fromPropertyWithKey:) for related information.

`NSDeleteCommand` is part of Cocoa’s built-in scripting support. Most applications don’t need to subclass `NSDeleteCommand` or call its methods.

## Topics

### Working with specifiers

var keySpecifier: NSScriptObjectSpecifier

Returns a specifier for the object or objects to be deleted.

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

class NSMoveCommand

A command that moves one or more scriptable objects.

class NSCreateCommand

A command that creates a scriptable object.

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

