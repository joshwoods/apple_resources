

- Core Data
- NSManagedObjectModel
-  entitiesByName 

Instance Property

# entitiesByName

The entities of the model, keyed by name.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var entitiesByName: [String : NSEntityDescription] { get }
```

## Discussion

Entities are instances of NSEntityDescription.

## See Also

### Related Documentation

class func entity(forEntityName: String, in: NSManagedObjectContext) -> NSEntityDescription?

Returns the entity with the specified name from the managed object model associated with the specified managed object context’s persistent store coordinator.

### Managing entities and configurations

var entities: [NSEntityDescription]

The entities in the model.

var configurations: [String]

All the available configuration names of the model.

func entities(forConfigurationName: String?) -> [NSEntityDescription]?

Returns the entities of the model for a specified configuration.

func setEntities([NSEntityDescription], forConfigurationName: String)

Associates the specified entities with the model using the given configuration name.

