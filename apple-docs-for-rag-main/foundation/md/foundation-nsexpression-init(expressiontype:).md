

- Foundation
- NSExpression
-  init(expressionType:) 

Initializer

# init(expressionType:)

Creates the expression with the specified expression type.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(expressionType type: NSExpression.ExpressionType)
```

## Parameters 

`type`  

The type of the new expression, as defined by NSExpression.ExpressionType.

## Return Value

An initialized `NSExpression` object of the type `type`.

## Discussion

This method is the designated initializer for `NSExpression`.

## See Also

### Related Documentation

Predicate Programming Guide

### Creating an Expression

init(format: String, argumentArray: [Any])

Creates the expression with the specified expression format and array of arguments.

init(format: String, arguments: CVaListPointer)

Creates the expression with the specified expression format and arguments list.

convenience init(format: String, any CVarArg...)

Creates the expression with the expression format and arguments list you specify.

init?(coder: NSCoder)

Creates an expression by decoding from the coder you specify.

