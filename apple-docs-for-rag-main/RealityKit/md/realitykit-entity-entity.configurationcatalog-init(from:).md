

- RealityKit
- Entity
- Entity.ConfigurationCatalog
-  init(from:) 

Initializer

# init(from:)

Loads a configuration catalog from a USD or reality file.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(from url: URL) async throws
```

## Parameters 

`url`  

A URL of a USD or `.reality` file.

## Discussion

This method parses a USD or `.reality` file, and provides a collection of available configurations based on USD variant sets or `.reality` file configurations. It doesn’t load large asset files, such as textures and meshes.

You can load an entity, and its assets, with configuration choices by calling init(from:configurations:).

