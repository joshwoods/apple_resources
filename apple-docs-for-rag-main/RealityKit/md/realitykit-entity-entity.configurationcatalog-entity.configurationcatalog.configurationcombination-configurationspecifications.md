

- RealityKit
- Entity
- Entity.ConfigurationCatalog
- Entity.ConfigurationCatalog.ConfigurationCombination
-  configurationSpecifications 

Instance Property

# configurationSpecifications

A dictionary that associates IDs of configuration sets to IDs of configurations.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
let configurationSpecifications: [String : String]
```

## Discussion

Use this property to represent a configuration choice from each configuration set.

## See Also

### Accessing values

let entity: Entity

The entity that represents the configuration choices.

