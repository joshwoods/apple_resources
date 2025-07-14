

- Core Data
- NSEntityMapping
-  mappingType 

Instance Property

# mappingType

The mapping type for the entity mapping.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var mappingType: NSEntityMappingType { get set }
```

## Discussion

If you specify a custom entity mapping type, you must specify a value for the migration policy class name as well (see entityMigrationPolicyClassName).

## See Also

### Managing Mapping Information

var name: String!

The name of the entity mapping.

var entityMigrationPolicyClassName: String?

The class name of the migration policy for the entity mapping.

var attributeMappings: [NSPropertyMapping]?

The array of attribute mappings for the entity mapping.

var relationshipMappings: [NSPropertyMapping]?

The array of relationship mappings for the entity mapping.

var userInfo: [AnyHashable : Any]?

The user info dictionary for the entity mapping.

