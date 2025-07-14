

- RealityKit
- Entity
- Entity.ConfigurationCatalog
-  init(configurationSets:combinations:) 

Initializer

# init(configurationSets:combinations:)

Creates a configuration catalog from in-memory entities and a dictionary of configuration sets.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    configurationSets: [String : Entity.ConfigurationCatalog.ConfigurationSet],
    combinations: [Entity.ConfigurationCatalog.ConfigurationCombination]
) throws
```

## Parameters 

`configurationSets`  

The configuration choices that the configuration catalog presents. Each key needs to match the ID of the configuration set value it maps to.

`combinations`  

The combinations of in-memory entities and configurations that can address them. The keys you use in configurationSpecifications need to match IDs of configuration sets from the `configurationSets` argument. The values you use in configurationSpecifications need to match IDs of configurations from the `configurationSets` argument. There needs to be one Entity.ConfigurationCatalog.ConfigurationCombination for each possible combination of configurations.

## Return Value

A configuration catalog that maintains the provided entities in memory.

## See Also

### Creating a configuration catalog from entities

init(configurationSets: [Entity.ConfigurationCatalog.ConfigurationSet], combinations: [Entity.ConfigurationCatalog.ConfigurationCombination]) throws

Creates a configuration catalog from in-memory entities and an array of configuration sets.

