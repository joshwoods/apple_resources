

- System
- FilePath
-  init(root:\_:) 

Initializer

# init(root:\_:)

Create a file path from a root and a collection of components.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    root: FilePath.Root?,
    _ components: C
) where C : Collection, C.Element == FilePath.Component
```

