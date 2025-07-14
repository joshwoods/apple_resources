

- Foundation
-  NSScriptCoercionHandler 

Class

# NSScriptCoercionHandler

A mechanism for converting one kind of scripting data to another.

Mac Catalyst 13.0+macOS 10.0+

``` source
class NSScriptCoercionHandler
```

## Overview

A shared instance of this class coerces (converts) object values to objects of another class using information supplied by classes that register with it. Coercions frequently are required during key-value coding.

## Topics

### Accessing the application’s handler

class func shared() -> NSScriptCoercionHandler

Returns the shared `NSScriptCoercionHandler` for the application.

### Working with handlers

func coerceValue(Any, to: AnyClass) -> Any?

Returns an object of a given class representing a given value.

func registerCoercer(Any, selector: Selector, toConvertFrom: AnyClass, to: AnyClass)

Registers a given object (typically a class) to handle coercions (conversions) from one given class to another.

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

class NSScriptExecutionContext

The context in which the current script command is executed.

