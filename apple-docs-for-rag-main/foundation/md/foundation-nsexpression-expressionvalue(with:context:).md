

- Foundation
- NSExpression
-  expressionValue(with:context:) 

Instance Method

# expressionValue(with:context:)

Evaluates an expression using a specified object and context.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func expressionValue(
    with object: Any?,
    context: NSMutableDictionary?
) -> Any?
```

## Parameters 

`object`  

The object against which the expression is evaluated.

`context`  

A dictionary that the expression can use to store temporary state for one predicate evaluation. Can be `nil`.

Note that `context` is mutable, and that it can only be accessed during the evaluation of the expression. You must not attempt to retain it for use elsewhere.

## Return Value

The evaluated object.

## See Also

### Evaluating an Expression

func allowEvaluation()

Forces a securely decoded expression to allow evaluation.

var `false`: NSExpression

An expression to evalutate if a conditional expression’s predicate evaluates to false.

var `true`: NSExpression

An expression to evalutate if a conditional expression’s predicate evaluates to true.

