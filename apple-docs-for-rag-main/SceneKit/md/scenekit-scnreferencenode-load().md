

- SceneKit
- SCNReferenceNode
-  load() 

Instance Method

# load()

Loads content into the node from its referenced external scene file.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@MainActor
func load()
```

**macOS, watchOS**

``` source
func load()
```

## Discussion

When SceneKit loads the referenced scene file, all children of the scene file’s root node become children of the reference node.

If the node has already been loaded (either automatically, according to the loadingPolicy property, or through a previous call to this method), calling this method has no effect.

## See Also

### Loading and Unloading a Reference Node’s Content

var referenceURL: URL

The URL to a scene file from which to load content for the reference node.

var loadingPolicy: SCNReferenceLoadingPolicy

An option for whether to load the node’s content automatically.

var isLoaded: Bool

A Boolean value that indicates whether the reference node has already loaded its content.

func unload()

Removes the node’s children and marks the node as not loaded.

