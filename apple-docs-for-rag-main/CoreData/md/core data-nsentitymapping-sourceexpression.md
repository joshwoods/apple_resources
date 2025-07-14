

- Core Data
- NSEntityMapping
-  sourceExpression 

Instance Property

# sourceExpression

The source expression for the entity mapping.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var sourceExpression: NSExpression? { get set }
```

## Discussion

The source expression is used to obtain the collection of managed objects to process through the mapping. The expression can be a fetch request expression, or any other expression that evaluates to a collection.

## See Also

### Managing Source Information

var sourceEntityName: String?

The source entity name for the entity mapping.

var sourceEntityVersionHash: Data?

The version hash of the source entity for the entity mapping.

