

- SceneKit
- SCNReferenceNode
-  init(url:) 

Initializer

# init(url:)

Initializes a node whose content is to be loaded from the referenced URL.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@MainActor
init?(url referenceURL: URL)
```

**macOS, watchOS**

``` source
init?(url referenceURL: URL)
```

## Parameters 

`referenceURL`  

The URL to a scene file from which to load the node’s content.

## Return Value

A new reference node.

## Discussion

Using this initializer does not load the node’s content. To load content from the referenced URL, use the load() method.

