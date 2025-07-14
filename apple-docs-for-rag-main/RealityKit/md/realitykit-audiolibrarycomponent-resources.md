

- RealityKit
- AudioLibraryComponent
-  resources 

Instance Property

# resources

A dictionary of audio resources with user-defined names.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var resources: [String : AudioResource]
```

## Discussion

The values can be any AudioResource type, such as AudioFileResource or AudioFileGroupResource. In memory, you can also use AudioBufferResource, but this type doesn’t support serializing to disk or sharing via network.

