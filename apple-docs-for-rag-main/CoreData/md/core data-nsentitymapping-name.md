

- Core Data
- NSEntityMapping
-  name 

Instance Property

# name

The name of the entity mapping.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var name: String! { get set }
```

## Discussion

The name is used only as a means of distinguishing mappings in a model. If not specified, the value defaults to SOURCE-\>DESTINATION.

## See Also

### Managing Mapping Information

var mappingType: NSEntityMappingType

The mapping type for the entity mapping.

var entityMigrationPolicyClassName: String?

The class name of the migration policy for the entity mapping.

var attributeMappings: [NSPropertyMapping]?

The array of attribute mappings for the entity mapping.

var relationshipMappings: [NSPropertyMapping]?

The array of relationship mappings for the entity mapping.

var userInfo: [AnyHashable : Any]?

The user info dictionary for the entity mapping.

