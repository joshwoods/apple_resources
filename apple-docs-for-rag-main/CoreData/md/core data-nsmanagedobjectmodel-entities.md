

- Core Data
- NSManagedObjectModel
-  entities 

Instance Property

# entities

The entities in the model.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var entities: [NSEntityDescription] { get set }
```

## Discussion

Entities are instances of NSEntityDescription.

### Special Considerations

Setting the entities for an object model raises an exception if the object model has been used by an object graph manager.

## See Also

### Managing entities and configurations

var entitiesByName: [String : NSEntityDescription]

The entities of the model, keyed by name.

var configurations: [String]

All the available configuration names of the model.

func entities(forConfigurationName: String?) -> [NSEntityDescription]?

Returns the entities of the model for a specified configuration.

func setEntities([NSEntityDescription], forConfigurationName: String)

Associates the specified entities with the model using the given configuration name.

