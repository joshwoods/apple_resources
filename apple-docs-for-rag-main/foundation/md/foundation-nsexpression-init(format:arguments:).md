

- Foundation
- NSExpression
-  init(format:arguments:) 

Initializer

# init(format:arguments:)

Creates the expression with the specified expression format and arguments list.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    format expressionFormat: String,
    arguments argList: CVaListPointer
)
```

## Parameters 

`expressionFormat`  

The expression format.

`argList`  

A list of arguments to be inserted into the `expressionFormat` string. The argument list is terminated by `nil`.

## Return Value

An initialized `NSExpression` object with the specified arguments.

## See Also

### Creating an Expression

init(expressionType: NSExpression.ExpressionType)

Creates the expression with the specified expression type.

init(format: String, argumentArray: [Any])

Creates the expression with the specified expression format and array of arguments.

convenience init(format: String, any CVarArg...)

Creates the expression with the expression format and arguments list you specify.

init?(coder: NSCoder)

Creates an expression by decoding from the coder you specify.

