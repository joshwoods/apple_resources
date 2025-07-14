

- Foundation
- NSSpecifierTest
-  init(objectSpecifier:comparisonOperator:test:) 

Initializer

# init(objectSpecifier:comparisonOperator:test:)

Returns a specifier test initialized to evaluate a test object against an object specified by an object specifier using a given comparison operation.

Mac Catalyst 13.0+macOS 10.0+

``` source
init(
    objectSpecifier obj1: NSScriptObjectSpecifier?,
    comparisonOperator compOp: NSSpecifierTest.TestComparisonOperation,
    test obj2: Any?
)
```

## Parameters 

`obj1`  

An object specifier.

`compOp`  

The comparison operation.

`obj2`  

The object against which to evaluate the object specified by `obj1`.

## Return Value

A specifier test initialized to evaluate (`obj2`) against an object specified by `obj1` using the comparison operation `compOp`.

## See Also

### Related Documentation

Cocoa Scripting Guide

