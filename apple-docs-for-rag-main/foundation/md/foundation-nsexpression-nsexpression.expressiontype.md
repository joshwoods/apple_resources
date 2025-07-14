

- Foundation
- NSExpression
-  NSExpression.ExpressionType 

Enumeration

# NSExpression.ExpressionType

Defines the possible types of an expression.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum ExpressionType
```

## Topics

### Constants

case constantValue

An expression that always returns the same value.

case evaluatedObject

An expression that always returns the parameter object itself.

case variable

An expression that always returns whatever value is associated with the key specified by ‘variable’ in the bindings dictionary.

case keyPath

An expression that returns something that can be used as a key path.

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

case keyPath

An expression that returns something that can be used as a key path.

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

### Enumeration Cases

case conditional

case conditional

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting Information About an Expression

var arguments: [NSExpression]?

The arguments for the expression.

var collection: Any

The collection of expressions in an aggregate expression, or the collection element of a subquery expression.

var constantValue: Any?

The constant value of the expression.

var expressionType: NSExpression.ExpressionType

The expression type for the expression.

var function: String

The function for the expression.

var keyPath: String

The key path for the expression.

var operand: NSExpression

The operand for the expression.

var predicate: NSPredicate

The predicate of a subquery expression.

var left: NSExpression

The left expression of an aggregate expression.

var right: NSExpression

The right expression of an aggregate expression.

var variable: String

The variable for the expression.

