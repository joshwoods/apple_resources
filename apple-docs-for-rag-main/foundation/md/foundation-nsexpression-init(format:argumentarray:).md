

- Foundation
- NSExpression
-  init(format:argumentArray:) 

Initializer

# init(format:argumentArray:)

Creates the expression with the specified expression format and array of arguments.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    format expressionFormat: String,
    argumentArray arguments: [Any]
)
```

## Parameters 

`expressionFormat`  

The expression format.

`arguments`  

An array of arguments to be used with the `expressionFormat` string.

## Return Value

An initialized `NSExpression` object with the specified arguments.

## See Also

### Creating an Expression

init(expressionType: NSExpression.ExpressionType)

Creates the expression with the specified expression type.

init(format: String, arguments: CVaListPointer)

Creates the expression with the specified expression format and arguments list.

convenience init(format: String, any CVarArg...)

Creates the expression with the expression format and arguments list you specify.

init?(coder: NSCoder)

Creates an expression by decoding from the coder you specify.

