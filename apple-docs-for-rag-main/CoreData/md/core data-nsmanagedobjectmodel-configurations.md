

- Core Data
- NSManagedObjectModel
-  configurations 

Instance Property

# configurations

All the available configuration names of the model.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var configurations: [String] { get }
```

## See Also

### Managing entities and configurations

var entities: [NSEntityDescription]

The entities in the model.

var entitiesByName: [String : NSEntityDescription]

The entities of the model, keyed by name.

func entities(forConfigurationName: String?) -> [NSEntityDescription]?

Returns the entities of the model for a specified configuration.

func setEntities([NSEntityDescription], forConfigurationName: String)

Associates the specified entities with the model using the given configuration name.

