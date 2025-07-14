

- Foundation
-  NSSpecifierTest 

Class

# NSSpecifierTest

A comparison between an object specifier and a test object.

Mac Catalyst 13.0+macOS 10.0+

``` source
class NSSpecifierTest
```

## Overview

Instances of this class represent a Boolean expression; they evaluate an object specifier and compare the resulting object to another object using a given comparison method. For more information on `NSSpecifierTest`, see the method description for its sole public method, its initializer, init(objectSpecifier:comparisonOperator:test:).

When an `NSSpecifierTest` object is properly initialized, it holds two objects:

- A “value” or “test” object used as the basis of the comparison; this object can be a regular object or object specifier (such as “blue” in “words whose color is blue”).

- An object specifier evaluating to the container (“words”).

The instance also encapsulates a selector identifying the method performing this comparison. The informal protocol NSComparisonMethods defines a set of comparison methods useful for this purpose, while NSScriptingComparisonMethods describes additional methods you may need to use for scripting.

The test object is compared, using the selector, against each object in the container. Specifiers in these tests usually have containerIsObjectBeingTested invoked on their topmost container.

You should rarely need to subclass `NSSpecifierTest`.

## Topics

### Initializing a specifier test

init(objectSpecifier: NSScriptObjectSpecifier?, comparisonOperator: NSSpecifierTest.TestComparisonOperation, test: Any?)

Returns a specifier test initialized to evaluate a test object against an object specified by an object specifier using a given comparison operation.

### Constants

enum TestComparisonOperation

These are passed to init(objectSpecifier:comparisonOperator:test:) to specify the comparison operator.

### Initializers

init?(coder: NSCoder)

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

class NSLogicalTest

The logical combination of one or more specifier tests.

