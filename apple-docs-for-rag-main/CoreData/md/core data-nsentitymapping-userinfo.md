

- Core Data
- NSEntityMapping
-  userInfo 

Instance Property

# userInfo

The user info dictionary for the entity mapping.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var userInfo: [AnyHashable : Any]? { get set }
```

## Discussion

You can use the info dictionary in any way that might be useful in your migration. You can set the contents of the dictionary directory or using the appropriate inspector in the Xcode mapping model editor.

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

var relationshipMappings: [NSPropertyMapping]?

The array of relationship mappings for the entity mapping.

