

- Foundation
- NSExpression
-  allowEvaluation() 

Instance Method

# allowEvaluation()

Forces a securely decoded expression to allow evaluation.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func allowEvaluation()
```

## Discussion

When securely decoding an `NSExpression` object encoded using NSSecureCoding, evaluation is disabled because it is potentially unsafe to evaluate expressions you get out of an archive.

Before you enable evaluation, you should validate key paths, selectors, etc to ensure no erroneous or malicious code will be executed. Once you’ve preflighted the expression, you can enable the expression for evaluation by calling `allowEvaluation`.

## See Also

### Evaluating an Expression

func expressionValue(with: Any?, context: NSMutableDictionary?) -> Any?

Evaluates an expression using a specified object and context.

var `false`: NSExpression

An expression to evalutate if a conditional expression’s predicate evaluates to false.

var `true`: NSExpression

An expression to evalutate if a conditional expression’s predicate evaluates to true.

