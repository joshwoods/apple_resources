

- Foundation
- NSExpression
-  expressionForEvaluatedObject() 

Type Method

# expressionForEvaluatedObject()

Creates an expression that represents the object you’re evaluating.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func expressionForEvaluatedObject() -> NSExpression
```

## Return Value

A new expression that represents the object being evaluated.

## See Also

### Creating an Expression for a Value

init(forConstantValue: Any?)

Creates an expression that represents a specified constant value.

init(forKeyPath: String)

Creates an expression that invokes the value function with a specified key path.

init(forVariable: String)

Creates an expression that extracts a value from the variable bindings dictionary for a specified key.

convenience init&lt;Root, Value>(forKeyPath: KeyPath&lt;Root, Value>)

Creates an expression using a key path you specify.

class func expressionForAnyKey() -> NSExpression

Creates an expression that represents any key for a Spotlight query.

