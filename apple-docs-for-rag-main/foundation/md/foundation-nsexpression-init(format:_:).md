

- Foundation
- NSExpression
-  init(format:\_:) 

Initializer

# init(format:\_:)

Creates the expression with the expression format and arguments list you specify.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(
    format expressionFormat: String,
    _ args: any CVarArg...
)
```

## Parameters 

`expressionFormat`  

The expression format.

`args`  

A list of arguments to insert into the `expressionFormat` string.

## See Also

### Creating an Expression

init(expressionType: NSExpression.ExpressionType)

Creates the expression with the specified expression type.

init(format: String, argumentArray: [Any])

Creates the expression with the specified expression format and array of arguments.

init(format: String, arguments: CVaListPointer)

Creates the expression with the specified expression format and arguments list.

init?(coder: NSCoder)

Creates an expression by decoding from the coder you specify.

