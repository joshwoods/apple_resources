

- Foundation
- NSExpression
-  init(forKeyPath:) 

Initializer

# init(forKeyPath:)

Creates an expression that invokes the value function with a specified key path.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(forKeyPath keyPath: String)
```

## Parameters 

`keyPath`  

The key path that the new expression should evaluate.

## Return Value

A new expression that invokes value(forKeyPath:) with `keyPath`.

## See Also

### Creating an Expression for a Value

init(forConstantValue: Any?)

Creates an expression that represents a specified constant value.

class func expressionForEvaluatedObject() -> NSExpression

Creates an expression that represents the object you’re evaluating.

init(forVariable: String)

Creates an expression that extracts a value from the variable bindings dictionary for a specified key.

convenience init&lt;Root, Value>(forKeyPath: KeyPath&lt;Root, Value>)

Creates an expression using a key path you specify.

class func expressionForAnyKey() -> NSExpression

Creates an expression that represents any key for a Spotlight query.

