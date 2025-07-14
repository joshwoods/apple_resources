

- Core Data
- NSManagedObjectModel
-  setEntities(\_:forConfigurationName:) 

Instance Method

# setEntities(\_:forConfigurationName:)

Associates the specified entities with the model using the given configuration name.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func setEntities(
    _ entities: [NSEntityDescription],
    forConfigurationName configuration: String
)
```

## Parameters 

`entities`  

An array of instances of `NSEntityDescription`.

`configuration`  

A name for the configuration.

## Discussion

This method raises an exception if the receiver has been used by an object graph manager.

## See Also

### Managing entities and configurations

var entities: [NSEntityDescription]

The entities in the model.

var entitiesByName: [String : NSEntityDescription]

The entities of the model, keyed by name.

var configurations: [String]

All the available configuration names of the model.

func entities(forConfigurationName: String?) -> [NSEntityDescription]?

Returns the entities of the model for a specified configuration.

