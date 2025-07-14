

- RealityKit
- Entity
- Entity.ConfigurationCatalog
- Entity.ConfigurationCatalog.ConfigurationSet
-  init(id:configurations:defaultConfigurationId:) 

Initializer

# init(id:configurations:defaultConfigurationId:)

Creates a configuration set from an ID, a dictionary of configurations, and a default configuration ID.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    id: String,
    configurations: [String : Entity.ConfigurationCatalog.Configuration],
    defaultConfigurationId: String? = nil
) throws
```

## Parameters 

`id`  

The ID of the configuration set that’s unique across all other configuration sets.

`configurations`  

A dictionary of configurations you can choose from. Each key needs to match the ID of the configuration value it maps to.

`defaultConfigurationId`  

The ID of one of the configuration elements in the `configurations` parameter, which is the default configuration the entity initializer applies if you don’t choose a configuration from the set.

## Return Value

A configuration set containing the configurations.

## See Also

### Creating a configuration set

init(id: String, configurations: [Entity.ConfigurationCatalog.Configuration], defaultConfigurationId: String?) throws

Creates a configuration set from an ID, an array of configurations, and a default configuration ID.

