

- RealityKit
- RealityViewAttachmentBuilderContent
-  transformEnvironment(\_:transform:) 

Instance Method

# transformEnvironment(\_:transform:)

Transforms the environment value of the specified key path with the given function.

RealityKitSwiftUIiOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
nonisolated
func transformEnvironment(
    _ keyPath: WritableKeyPath,
    transform: @escaping (inout V) -> Void
) -> some View
```

