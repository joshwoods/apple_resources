

- RealityKit
- Entity
-  init(from:configurations:) 

Initializer

# init(from:configurations:)

Loads an entity from a configuration catalog and a dictionary of configuration choices.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor @preconcurrency
convenience init(
    from catalog: Entity.ConfigurationCatalog,
    configurations: [String : String]? = nil
) async throws
```

## Parameters 

`catalog`  

A collection of alternative representations for an entity.

`configurations`  

A dictionary of configuration choices the initializer applies as it loads the entity, mapping the ID of a configuration set to the ID of a configuration within that set.

## See Also

### Loading an entity from a configuration catalog

struct ConfigurationCatalog

A collection of alternative representations of an entity you can choose from.

