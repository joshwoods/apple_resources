

- Foundation
-  NSScriptWhoseTest 

Class

# NSScriptWhoseTest

An abstract class that provides the basis for testing specifiers one at a time or in groups.

Mac Catalyst 13.0+macOS 10.0+

``` source
class NSScriptWhoseTest
```

## Overview

`NSScriptWhoseTest` is an abstract class whose sole method is isTrue(). Two concrete subclasses of `NSScriptWhoseTest` generate objects representing Boolean expressions comparing one object with another and objects representing multiple Boolean expressions connected by logical operators (`OR`, `AND`, `NOT`). These classes are, respectively, NSSpecifierTest and NSLogicalTest. In evaluating itself, an NSWhoseSpecifier invokes the isTrue() method of its “test” object.

You shouldn’t need to subclass `NSScriptWhoseTest`, and you should rarely need to subclass one of its subclasses.

## Topics

### Evaluating a test

func isTrue() -> Bool

Returns a Boolean value that indicates whether the test represented by the receiver evaluates to true.

### Initializers

init()

init?(coder: NSCoder)

## Relationships

### Inherits From

- NSObject

### Inherited By

- NSLogicalTest
- NSSpecifierTest

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

class NSSpecifierTest

A comparison between an object specifier and a test object.

class NSLogicalTest

The logical combination of one or more specifier tests.

