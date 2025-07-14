

- SceneKit
- SCNReferenceNode
-  isLoaded 

Instance Property

# isLoaded

A Boolean value that indicates whether the reference node has already loaded its content.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@MainActor
var isLoaded: Bool { get }
```

**macOS, watchOS**

``` source
var isLoaded: Bool { get }
```

## See Also

### Loading and Unloading a Reference Node’s Content

var referenceURL: URL

The URL to a scene file from which to load content for the reference node.

var loadingPolicy: SCNReferenceLoadingPolicy

An option for whether to load the node’s content automatically.

func load()

Loads content into the node from its referenced external scene file.

func unload()

Removes the node’s children and marks the node as not loaded.

