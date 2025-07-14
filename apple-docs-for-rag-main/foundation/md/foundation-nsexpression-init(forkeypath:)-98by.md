

- Foundation
- NSExpression
-  init(forKeyPath:) 

Initializer

# init(forKeyPath:)

Creates an expression using a key path you specify.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(forKeyPath keyPath: KeyPath)
```

## Parameters 

`keyPath`  

The key path that the new expression evaluates.

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

class func expressionForAnyKey() -> NSExpression

Creates an expression that represents any key for a Spotlight query.

