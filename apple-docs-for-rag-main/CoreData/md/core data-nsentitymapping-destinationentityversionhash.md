

- Core Data
- NSEntityMapping
-  destinationEntityVersionHash 

Instance Property

# destinationEntityVersionHash

The version hash for the destination entity for the entity mapping.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var destinationEntityVersionHash: Data? { get set }
```

## Discussion

The version hash is calculated by Core Data based on the property values of the entity (see `NSEntityDescription`’s versionHash method). The `destinationEntityVersionHash` must equal the version hash of the destination entity represented by the mapping.

## See Also

### Related Documentation

var sourceEntityVersionHash: Data?

The version hash of the source entity for the entity mapping.

### Managing Destination Information

var destinationEntityName: String?

The destination entity name for the entity mapping.

