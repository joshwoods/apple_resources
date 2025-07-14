

- Foundation
- NSExpression
-  expressionBlock 

Instance Property

# expressionBlock

The block that executes to evaluate the expression.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var expressionBlock: (Any?, [NSExpression], NSMutableDictionary?) -> Any { get }
```

## See Also

### Related Documentation

init(block: (Any?, [NSExpression], NSMutableDictionary?) -> Any, arguments: [NSExpression]?)

Creates an expression object that uses the block for evaluating objects.

