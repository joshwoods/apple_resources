

- Foundation
-  NSLogicalTest 

Class

# NSLogicalTest

The logical combination of one or more specifier tests.

Mac Catalyst 13.0+macOS 10.0+

``` source
class NSLogicalTest
```

## Overview

Instances of this class perform logical operations of `AND`, `OR`, and `NOT` on Boolean expressions represented by NSSpecifierTest objects. These operators are equivalent to “`&&`”, “`||`”, and “`!`” in the C language.

For `AND` and `OR` operations, an `NSLogicalTest` object is typically initialized with an array containing two or more NSSpecifierTest objects. isTrue()—inherited from NSScriptWhoseTest—evaluates the array in a manner appropriate to the logical operation. For `NOT` operations, an `NSLogicalTest` object is initialized with only one `NSSpecifierTest` object; it simply reverses the Boolean outcome of the isTrue() method.

You don’t normally subclass `NSLogicalTest`.

## Topics

### Initializing a logical test

init(andTestWith: [NSSpecifierTest])

Returns an `NSLogicalTest` object initialized to perform an `AND` operation with the `NSSpecifierTest` objects in a given array.

init(notTestWith: NSScriptWhoseTest)

Returns an `NSLogicalTest` object initialized to perform a `NOT` operation on the given `NSScriptWhoseTest` object.

init(orTestWith: [NSSpecifierTest])

Returns an `NSLogicalTest` object initialized to perform an `OR` operation with the `NSSpecifierTest` objects in a given array.

## Relationships

### Inherits From

- NSScriptWhoseTest

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol

## See Also

### Object Matching Tests

class NSScriptWhoseTest

An abstract class that provides the basis for testing specifiers one at a time or in groups.

class NSSpecifierTest

A comparison between an object specifier and a test object.

