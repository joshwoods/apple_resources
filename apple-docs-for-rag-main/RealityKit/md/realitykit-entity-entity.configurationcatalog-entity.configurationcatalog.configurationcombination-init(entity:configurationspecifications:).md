

- RealityKit
- Entity
- Entity.ConfigurationCatalog
- Entity.ConfigurationCatalog.ConfigurationCombination
-  init(entity:configurationSpecifications:) 

Initializer

# init(entity:configurationSpecifications:)

Creates a configuration combination from an entity and a configuration dictionary.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    entity: Entity,
    configurationSpecifications: [String : String]
)
```

## Parameters 

`entity`  

An entity that represents the configuration choices in `configurationSpecifications`.

`configurationSpecifications`  

A dictionary that associates a configuration set name with a choice from that set.

