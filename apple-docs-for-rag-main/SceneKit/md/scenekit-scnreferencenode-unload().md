

- SceneKit
- SCNReferenceNode
-  unload() 

Instance Method

# unload()

Removes the node’s children and marks the node as not loaded.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

**macOS, watchOS**

``` source
func unload()
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@MainActor
func unload()
```

## Discussion

Calling this method does not necessarily unload any content associated with the node’s child nodes from memory—it merely removes them from the scene graph. The unlinked nodes and their content are then subject to normal object memory management rules. Under ARC, those objects are deallocated if and only if they are not referenced from elsewhere in your program.

## See Also

### Loading and Unloading a Reference Node’s Content

var referenceURL: URL

The URL to a scene file from which to load content for the reference node.

var loadingPolicy: SCNReferenceLoadingPolicy

An option for whether to load the node’s content automatically.

func load()

Loads content into the node from its referenced external scene file.

var isLoaded: Bool

A Boolean value that indicates whether the reference node has already loaded its content.

