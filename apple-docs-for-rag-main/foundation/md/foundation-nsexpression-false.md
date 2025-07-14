

- Foundation
- NSExpression
-  false 

Instance Property

# false

An expression to evalutate if a conditional expression’s predicate evaluates to false.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@NSCopying
var `false`: NSExpression { get }
```

## Discussion

Accessing this property raises an exception if it isn’t applicable to the expression.

## See Also

### Evaluating an Expression

func expressionValue(with: Any?, context: NSMutableDictionary?) -> Any?

Evaluates an expression using a specified object and context.

func allowEvaluation()

Forces a securely decoded expression to allow evaluation.

var `true`: NSExpression

An expression to evalutate if a conditional expression’s predicate evaluates to true.

