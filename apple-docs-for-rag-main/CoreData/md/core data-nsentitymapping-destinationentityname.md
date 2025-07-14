

- Core Data
- NSEntityMapping
-  destinationEntityName 

Instance Property

# destinationEntityName

The destination entity name for the entity mapping.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var destinationEntityName: String? { get set }
```

## Discussion

Mappings are not directly bound to entity descriptions. You can use the migration manager’s destinationEntity(for:) method to retrieve the entity description for this entity name.

## See Also

### Related Documentation

var sourceEntityName: String?

The source entity name for the entity mapping.

### Managing Destination Information

var destinationEntityVersionHash: Data?

The version hash for the destination entity for the entity mapping.

