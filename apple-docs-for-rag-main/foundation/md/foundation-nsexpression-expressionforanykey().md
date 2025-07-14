

- Foundation
- NSExpression
-  expressionForAnyKey() 

Type Method

# expressionForAnyKey()

Creates an expression that represents any key for a Spotlight query.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func expressionForAnyKey() -> NSExpression
```

## Return Value

A new expression that represents any key for a Spotlight query.

## See Also

### Creating an Expression for a Value

init(forConstantValue: Any?)

Creates an expression that represents a specified constant value.

class func expressionForEvaluatedObject() -> NSExpression

Creates an expression that represents the object you’re evaluating.

init(forKeyPath: String)

Creates an expression that invokes the value function with a specified key path.

init(forVariable: String)

Creates an expression that extracts a value from the variable bindings dictionary for a specified key.

convenience init&lt;Root, Value>(forKeyPath: KeyPath&lt;Root, Value>)

Creates an expression using a key path you specify.

