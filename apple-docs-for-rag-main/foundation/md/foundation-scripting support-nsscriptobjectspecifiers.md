

- Foundation
- Scripting Support
-  NSScriptObjectSpecifiers 

# NSScriptObjectSpecifiers

A collection of methods providing additional object specifier functionality.

## Overview

These methods allow scriptable objects to provide a fully specified object specifier to themselves within an app. They also enable containers of objects to perform their own specifier evaluation.

For a comprehensive treatment of object specifiers, including sample code, see Object Specifiers in Cocoa Scripting Guide.

## Topics

### Working with object specifiers

var objectSpecifier: NSScriptObjectSpecifier? { get }

Returns an object specifier for the receiver.

func indicesOfObjects(byEvaluatingObjectSpecifier specifier: NSScriptObjectSpecifier) -> [NSNumber]?

Returns the indices of the specified container objects.

## See Also

### Related Documentation

Cocoa Scripting Guide

### NSObject Script Support

NSComparisonMethods

A collection of default comparison methods useful for performing specifier tests.

NSScriptingComparisonMethods

A collection of methods useful for comparing script objects.

NSScriptKeyValueCoding

A collection of methods that provide additional capabilities for working with key-value coding.

class NSScriptCoercionHandler

A mechanism for converting one kind of scripting data to another.

class NSScriptExecutionContext

The context in which the current script command is executed.

