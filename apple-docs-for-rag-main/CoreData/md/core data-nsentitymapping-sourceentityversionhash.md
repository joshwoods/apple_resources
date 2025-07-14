

- Core Data
- NSEntityMapping
-  sourceEntityVersionHash 

Instance Property

# sourceEntityVersionHash

The version hash of the source entity for the entity mapping.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var sourceEntityVersionHash: Data? { get set }
```

## Discussion

The version hash is calculated by Core Data based on the property values of the entity (see `NSEntityDescription`’s versionHash method). The `sourceEntityVersionHash` must equal the version hash of the source entity represented by the mapping.

## See Also

### Related Documentation

var destinationEntityVersionHash: Data?

The version hash for the destination entity for the entity mapping.

### Managing Source Information

var sourceEntityName: String?

The source entity name for the entity mapping.

var sourceExpression: NSExpression?

The source expression for the entity mapping.

