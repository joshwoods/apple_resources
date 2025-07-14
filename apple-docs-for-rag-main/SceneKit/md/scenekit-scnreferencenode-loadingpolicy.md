

- SceneKit
- SCNReferenceNode
-  loadingPolicy 

Instance Property

# loadingPolicy

An option for whether to load the node’s content automatically.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

**macOS, watchOS**

``` source
var loadingPolicy: SCNReferenceLoadingPolicy { get set }
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@MainActor
var loadingPolicy: SCNReferenceLoadingPolicy { get set }
```

## Discussion

If this property’s value is SCNReferenceLoadingPolicy.immediate (the default), instantiating a reference node from an archive (using the NSKeyedUnarchiver class) automatically loads the node’s external content. Set this property to SCNReferenceLoadingPolicy.onDemand before archiving an SCNReferenceNode object if you don’t want that reference node to automatically load its content when unarchived. In that case, call the load() method after unarchiving when you want to load the node’s content.

## See Also

### Loading and Unloading a Reference Node’s Content

var referenceURL: URL

The URL to a scene file from which to load content for the reference node.

func load()

Loads content into the node from its referenced external scene file.

var isLoaded: Bool

A Boolean value that indicates whether the reference node has already loaded its content.

func unload()

Removes the node’s children and marks the node as not loaded.

