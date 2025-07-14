

- Core Data
- NSManagedObjectModel
-  entities(forConfigurationName:) 

Instance Method

# entities(forConfigurationName:)

Returns the entities of the model for a specified configuration.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func entities(forConfigurationName configuration: String?) -> [NSEntityDescription]?
```

## Parameters 

`configuration`  

The name of a configuration in the receiver.

## Return Value

An array containing the entities of the receiver for the configuration specified by `configuration`.

## See Also

### Managing entities and configurations

var entities: [NSEntityDescription]

The entities in the model.

var entitiesByName: [String : NSEntityDescription]

The entities of the model, keyed by name.

var configurations: [String]

All the available configuration names of the model.

func setEntities([NSEntityDescription], forConfigurationName: String)

Associates the specified entities with the model using the given configuration name.

