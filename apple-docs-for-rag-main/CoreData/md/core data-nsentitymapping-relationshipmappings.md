

- Core Data
- NSEntityMapping
-  relationshipMappings 

Instance Property

# relationshipMappings

The array of relationship mappings for the entity mapping.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var relationshipMappings: [NSPropertyMapping]? { get set }
```

## Discussion

The order of mappings in the array specifies the order in which the mappings will be processed during a migration.

## See Also

### Managing Mapping Information

var name: String!

The name of the entity mapping.

var mappingType: NSEntityMappingType

The mapping type for the entity mapping.

var entityMigrationPolicyClassName: String?

The class name of the migration policy for the entity mapping.

var attributeMappings: [NSPropertyMapping]?

The array of attribute mappings for the entity mapping.

var userInfo: [AnyHashable : Any]?

The user info dictionary for the entity mapping.

