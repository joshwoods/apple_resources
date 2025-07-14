

- Foundation
-  NSScriptCommand 

Class

# NSScriptCommand

A self-contained scripting statement.

Mac Catalyst 13.0+macOS 10.0+

``` source
class NSScriptCommand
```

## Overview

An instance of NSScriptCommand represents a scripting statement, such as `set word 5 of the front document to word 1 of the second document`, and contains the information needed to perform the operation specified by the statement.

When an Apple event reaches a Cocoa application, Cocoa’s built-in scripting support transforms it into a script command (that is, an instance of `NSScriptCommand` or one of the subclasses provided by Cocoa scripting or by your application) and executes the command in the context of the application. Executing a command means either invoking the selector associated with the command on the object or objects designated to receive the command, or having the command perform its default implementation method (performDefaultImplementation()).

Your application most likely calls methods of `NSScriptCommand` to extract the command arguments. You do this either in the `performDefaultImplementation` method of a command subclass you have created, or in an object method designated as the selector to handle a particular command.

As part of Cocoa’s standard scripting implementation, `NSScriptCommand` and its subclasses can handle the default command set for AppleScript’s Standard suite for most applications without any subclassing. The Standard suite includes commands such as `copy`, `count`, `create`, `delete`, `exists`, and `move`, as well as common object classes such as `application`, `document`, and `window`.

For more information on working with script commands, see Script Commands in Cocoa Scripting Guide.

## Topics

### Initializing a script command

init(commandDescription: NSScriptCommandDescription)

Returns an a script command object initialized from the passed command description.

### Getting the current command

class func current() -> NSScriptCommand?

If a command is being executed in the current thread by Cocoa scripting’s built-in Apple event handling, return the command.

### Getting the Apple event

var appleEvent: NSAppleEventDescriptor?

If the receiver was constructed by Cocoa scripting’s built-in Apple event handling, returns the Apple event descriptor from which it was constructed.

### Executing the command

func execute() -> Any?

Executes the command if it is valid and returns the result, if any.

func performDefaultImplementation() -> Any?

Overridden by subclasses to provide a default implementation for the command represented by the receiver.

### Accessing receivers

var evaluatedReceivers: Any?

Returns the object or objects to which the command is to be sent (called both the “receivers” or “targets” of script commands).

var receiversSpecifier: NSScriptObjectSpecifier?

Sets the object specifier to `receiversSpec` that, when evaluated, indicates the receiver or receivers of the command.

### Accessing arguments

var arguments: [String : Any]?

Sets the arguments of the command to `args`.

var evaluatedArguments: [String : Any]?

Returns a dictionary containing the arguments of the command, evaluated from object specifiers to objects if necessary. The keys in the dictionary are the argument names.

### Accessing the direct parameter

var directParameter: Any?

Sets the object that corresponds to the direct parameter of the Apple event from which the receiver derives.

### Getting command information

var commandDescription: NSScriptCommandDescription

Returns the command description for the command.

var isWellFormed: Bool

Returns a Boolean value indicating whether the receiver is well formed according to its command description.

### Handling script execution errors

var scriptErrorExpectedTypeDescriptor: NSAppleEventDescriptor?

Sets a descriptor for the expected type that will be put in the reply Apple event if the sender requested a reply, execution of the receiver completes, and an error number was set.

var scriptErrorNumber: Int

Sets a script error number that is associated with the execution of the command and is returned in the reply Apple event, if a reply was requested by the sender.

var scriptErrorOffendingObjectDescriptor: NSAppleEventDescriptor?

Sets a descriptor for an object that will be put in the reply Apple event if the sender requested a reply, execution of the receiver completes, and an error number was set.

var scriptErrorString: String?

Sets a script error string that is associated with execution of the command.

### Suspending and resuming commands

func suspendExecution()

Suspends the execution of the receiver.

func resumeExecution(withResult: Any?)

If a successful, unmatched, invocation of suspendExecution() has been made, resume the execution of the command.

### Constants

NSScriptCommand—General Command Execution Errors

`NSScriptCommand` uses the following error codes for general command execution problems:

### Initializers

convenience init?(coder: NSCoder)

## Relationships

### Inherits From

- NSObject

### Inherited By

- NSCloneCommand
- NSCloseCommand
- NSCountCommand
- NSCreateCommand
- NSDeleteCommand
- NSExistsCommand
- NSGetCommand
- NSMoveCommand
- NSQuitCommand
- NSSetCommand

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

class NSCloseCommand

A command that closes one or more scriptable objects.

