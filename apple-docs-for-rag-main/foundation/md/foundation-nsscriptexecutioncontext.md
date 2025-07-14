

- Foundation
-  NSScriptExecutionContext 

Class

# NSScriptExecutionContext

The context in which the current script command is executed.

Mac Catalyst 13.0+macOS 10.0+

``` source
class NSScriptExecutionContext
```

## Overview

An `NSScriptExecutionContext` object is a shared instance (there is only one instance of the class) that represents the context in which the current script command is executed. `NSScriptExecutionContext` tracks global state relating to the command being executed, especially the top-level container object (that is, the container implied by a specifier object that specifies no container) used in an evaluation of an NSScriptObjectSpecifier object.

In most cases, the top-level container for a complete series of nested object specifiers is automatically set to the application object (`NSApp`), and you can get this object with the topLevelObject method. But you can also set this top-level container to something else (using topLevelObject) if the situation warrants it.

It is unlikely that you will need to subclass `NSScriptExecutionContext`.

## Topics

### Getting the current context

class func shared() -> NSScriptExecutionContext

Returns the shared `NSScriptExecutionContext` instance.

### Getting and setting the container object

var topLevelObject: Any?

Sets the top-level object for an object-specifier evaluation.

var objectBeingTested: Any?

Sets the top-level container object currently being tested in a “whose” qualifier to a given object.

var rangeContainerObject: Any?

Sets the top-level container object for a range-specifier evaluation to a give object.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

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

