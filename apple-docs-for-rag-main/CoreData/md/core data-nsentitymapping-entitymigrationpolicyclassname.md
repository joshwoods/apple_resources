

- Core Data
- NSEntityMapping
-  entityMigrationPolicyClassName 

Instance Property

# entityMigrationPolicyClassName

The class name of the migration policy for the entity mapping.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var entityMigrationPolicyClassName: String? { get set }
```

## Discussion

If not specified, the default migration class name is NSEntityMigrationPolicy. You can specify a subclass to provide custom behavior.

## See Also

### Managing Mapping Information

var name: String!

The name of the entity mapping.

var mappingType: NSEntityMappingType

The mapping type for the entity mapping.

var attributeMappings: [NSPropertyMapping]?

The array of attribute mappings for the entity mapping.

var relationshipMappings: [NSPropertyMapping]?

The array of relationship mappings for the entity mapping.

var userInfo: [AnyHashable : Any]?

The user info dictionary for the entity mapping.

