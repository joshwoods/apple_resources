

- Foundation
- NSExpression
- NSExpression.ExpressionType
-  NSExpression.ExpressionType.keyPath 

Case

# NSExpression.ExpressionType.keyPath

An expression that returns something that can be used as a key path.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case keyPath
```

## See Also

### Constants

case constantValue

An expression that always returns the same value.

case evaluatedObject

An expression that always returns the parameter object itself.

case variable

An expression that always returns whatever value is associated with the key specified by ‘variable’ in the bindings dictionary.

case function

An expression that returns the result of evaluating a function.

case unionSet

An expression that creates a union of the results of two nested expressions.

case intersectSet

An expression that creates an intersection of the results of two nested expressions.

case minusSet

An expression that combines two nested expression results by set subtraction.

case subquery

An expression that filters a collection using a subpredicate.

case aggregate

An expression that defines an aggregate of `NSExpression` objects.

case anyKey

An expression that represents any key.

case block

An expression that uses a Block.

case constantValue

An expression that always returns the same value.

case evaluatedObject

An expression that always returns the parameter object itself.

case variable

An expression that always returns whatever value is associated with the key specified by ‘variable’ in the bindings dictionary.

case function

An expression that returns the result of evaluating a function.

