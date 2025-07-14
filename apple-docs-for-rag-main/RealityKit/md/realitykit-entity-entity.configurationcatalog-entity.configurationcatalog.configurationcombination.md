

- RealityKit
- Entity
- Entity.ConfigurationCatalog
-  Entity.ConfigurationCatalog.ConfigurationCombination 

Structure

# Entity.ConfigurationCatalog.ConfigurationCombination

A type that associates an entity with a combination of configurations.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct ConfigurationCombination
```

## Topics

### Creating a configuration combination

init(entity: Entity, configurationSpecifications: [String : String])

Creates a configuration combination from an entity and a configuration dictionary.

### Accessing values

let entity: Entity

The entity that represents the configuration choices.

let configurationSpecifications: [String : String]

A dictionary that associates IDs of configuration sets to IDs of configurations.

## See Also

### Defining configuration choices

struct Configuration

A type that represents an alternative that you can choose.

struct ConfigurationSet

A collection of alternatives to choose from.

