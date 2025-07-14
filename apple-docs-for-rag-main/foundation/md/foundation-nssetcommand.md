

- Foundation
-  NSSetCommand 

Class

# NSSetCommand

A command that sets one or more attributes or relationships to one or more values.

Mac Catalyst 13.0+macOS 10.0+

``` source
class NSSetCommand
```

## Overview

An instance of `NSSetCommand` sets one or more attributes or relationships to one or more values; for example, it may set the (x, y) coordinates for a window’s position or set the name of a document.

`NSSetCommand` is part of Cocoa’s built-in scripting support. It works automatically to support the `set` command through key-value coding. Most applications don’t need to subclass `NSSetCommand` or call its methods.

`NSSetCommand` uses available scripting class descriptions to determine whether it should set a value for an attribute (or property), or set a value for all elements (to-many objects). For the latter, it invokes replaceValue(at:inPropertyWithKey:withValue:); for the former, it invokes setValue(_:forKey:) (or, if the receiver overrides takeValue(_:forKey:), it invokes that method, to support backward binary compatibility.)

For information on working with `set` commands, see Getting and Setting Properties and Elements in Cocoa Scripting Guide.

## Topics

### Working with specifiers

var keySpecifier: NSScriptObjectSpecifier

Returns a specifier that identifies the attribute or relationship that is to be set for the receiver of the `set` AppleScript command.

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

