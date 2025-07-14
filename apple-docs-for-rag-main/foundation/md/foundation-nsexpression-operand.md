

- Foundation
- NSExpression
-  operand 

Instance Property

# operand

The operand for the expression.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@NSCopying
var operand: NSExpression { get }
```

## Discussion

The operand for an expression is the object on which the expression’s selector or block will be invoked. The object is the result of evaluating a key path or one of the defined functions. Accessing this property raises an exception if it is not applicable to the expression.

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

enum ExpressionType

Defines the possible types of an expression.

var function: String

The function for the expression.

var keyPath: String

The key path for the expression.

var predicate: NSPredicate

The predicate of a subquery expression.

var left: NSExpression

The left expression of an aggregate expression.

var right: NSExpression

The right expression of an aggregate expression.

var variable: String

The variable for the expression.

