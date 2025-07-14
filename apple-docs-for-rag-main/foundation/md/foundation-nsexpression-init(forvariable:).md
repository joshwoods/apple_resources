

- Foundation
- NSExpression
-  init(forVariable:) 

Initializer

# init(forVariable:)

Creates an expression that extracts a value from the variable bindings dictionary for a specified key.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(forVariable string: String)
```

## Parameters 

`string`  

The key for the variable to extract from the variable bindings dictionary.

## Return Value

A new expression that extracts from the variable bindings dictionary the value for the key `string`.

## See Also

### Creating an Expression for a Value

init(forConstantValue: Any?)

Creates an expression that represents a specified constant value.

class func expressionForEvaluatedObject() -> NSExpression

Creates an expression that represents the object you’re evaluating.

init(forKeyPath: String)

Creates an expression that invokes the value function with a specified key path.

convenience init&lt;Root, Value>(forKeyPath: KeyPath&lt;Root, Value>)

Creates an expression using a key path you specify.

class func expressionForAnyKey() -> NSExpression

Creates an expression that represents any key for a Spotlight query.

