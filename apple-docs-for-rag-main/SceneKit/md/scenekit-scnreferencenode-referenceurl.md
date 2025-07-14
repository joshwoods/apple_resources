

- SceneKit
- SCNReferenceNode
-  referenceURL 

Instance Property

# referenceURL

The URL to a scene file from which to load content for the reference node.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

**macOS, watchOS**

``` source
var referenceURL: URL { get set }
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@MainActor
var referenceURL: URL { get set }
```

## Discussion

When the reference node loads its content (either automatically, according to the loadingPolicy property, or when you call the load() method), SceneKit loads the referenced scene file. All children of the scene file’s root node become children of the reference node.

## See Also

### Loading and Unloading a Reference Node’s Content

var loadingPolicy: SCNReferenceLoadingPolicy

An option for whether to load the node’s content automatically.

func load()

Loads content into the node from its referenced external scene file.

var isLoaded: Bool

A Boolean value that indicates whether the reference node has already loaded its content.

func unload()

Removes the node’s children and marks the node as not loaded.

