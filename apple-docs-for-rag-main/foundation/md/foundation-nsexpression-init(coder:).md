

- Foundation
- NSExpression
-  init(coder:) 

Initializer

# init(coder:)

Creates an expression by decoding from the coder you specify.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(coder: NSCoder)
```

## Parameters 

`coder`  

The coder to read data from.

## See Also

### Creating an Expression

init(expressionType: NSExpression.ExpressionType)

Creates the expression with the specified expression type.

init(format: String, argumentArray: [Any])

Creates the expression with the specified expression format and array of arguments.

init(format: String, arguments: CVaListPointer)

Creates the expression with the specified expression format and arguments list.

convenience init(format: String, any CVarArg...)

Creates the expression with the expression format and arguments list you specify.

