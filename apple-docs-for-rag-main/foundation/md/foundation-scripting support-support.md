

- Foundation
-  Scripting Support 

API Collection

# Scripting Support

Allow users to control your app with AppleScript and other automation technologies, or run scripts from within your app.

## Topics

### Script Execution

class NSAppleScript

An object that provides the ability to load, compile, and execute scripts.

### Apple Event Handling

class NSAppleEventDescriptor

A wrapper for the Apple event descriptor data type.

class NSAppleEventManager

A mechanism for registering handler routines for specific types of Apple events and dispatching events to those handlers.

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

class NSCloseCommand

A command that closes one or more scriptable objects.

### Object Specifiers

class NSScriptObjectSpecifier

An abstract class used to represent natural language expressions.

class NSPropertySpecifier

A specifier for a simple attribute value, a one-to-one relationship, or all elements of a to-many relationship.

class NSPositionalSpecifier

A specifier for an insertion point in a container relative to another object in the container.

class NSRandomSpecifier

A specifier for an arbitrary object in a collection or, if not a one-to-many relationship, the sole object.

class NSRangeSpecifier

A specifier for a range of objects in a container.

class NSUniqueIDSpecifier

A specifier for an object in a collection (or container) by unique ID.

class NSWhoseSpecifier

A specifier that indicates every object in a collection matching a condition.

class NSNameSpecifier

A specifier for an object in a collection (or container) by name.

class NSMiddleSpecifier

A specifier indicating the middle object in a collection or, if not a one-to-many relationship, the sole object.

class NSIndexSpecifier

A specifier representing an object in a collection (or container) with an index number.

class NSRelativeSpecifier

A specifier that indicates an object in a collection by its position relative to another object.

### Script Dictionary Description

class NSScriptSuiteRegistry

The top-level repository of scriptability information for an app at runtime.

class NSScriptClassDescription

A scriptable class that a macOS app supports.

class NSClassDescription

An abstract class that provides the interface for querying the relationships and properties of a class.

class NSScriptCommandDescription

A script command that a macOS app supports.

### Object Matching Tests

class NSScriptWhoseTest

An abstract class that provides the basis for testing specifiers one at a time or in groups.

class NSSpecifierTest

A comparison between an object specifier and a test object.

class NSLogicalTest

The logical combination of one or more specifier tests.

### NSObject Script Support

NSComparisonMethods

A collection of default comparison methods useful for performing specifier tests.

NSScriptingComparisonMethods

A collection of methods useful for comparing script objects.

NSScriptKeyValueCoding

A collection of methods that provide additional capabilities for working with key-value coding.

NSScriptObjectSpecifiers

A collection of methods providing additional object specifier functionality.

class NSScriptCoercionHandler

A mechanism for converting one kind of scripting data to another.

class NSScriptExecutionContext

The context in which the current script command is executed.

## See Also

### App Support

Task Management

Manage your app’s work and how it interacts with system services like Handoff and Shortcuts.

Resources

Access assets and other data bundled with your app.

Notifications

Design patterns for broadcasting information and for subscribing to broadcasts.

App Extension Support

Manage the interaction between an app extension and its hosting app.

Errors and Exceptions

Respond to problem situations in your interactions with APIs, and fine-tune your app for better debugging.

