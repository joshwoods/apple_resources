

- Core Data
- NSEntityMapping
-  sourceEntityName 

Instance Property

# sourceEntityName

The source entity name for the entity mapping.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var sourceEntityName: String? { get set }
```

## Discussion

Mappings are not directly bound to entity descriptions; you can use the sourceEntity(for:) method on the migration manager to retrieve the entity description for this entity name.

## See Also

### Related Documentation

Core Data Model Versioning and Data Migration Programming Guide

var destinationEntityName: String?

The destination entity name for the entity mapping.

### Managing Source Information

var sourceEntityVersionHash: Data?

The version hash of the source entity for the entity mapping.

var sourceExpression: NSExpression?

The source expression for the entity mapping.

