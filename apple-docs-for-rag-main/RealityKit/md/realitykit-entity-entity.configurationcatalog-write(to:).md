

- RealityKit
- Entity
- Entity.ConfigurationCatalog
-  write(to:) 

Instance Method

# write(to:)

Writes the configurations of the configuration catalog to a reality file.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor
func write(to url: URL) async throws
```

## Parameters 

`url`  

The destination where the configuration catalog writes the `.reality` file.

## Discussion

Another configuration catalog instance can open the `.reality` file for reading.

