

- SpriteKit
- SKReferenceNode
-  didLoad(\_:) 

Instance Method

# didLoad(\_:)

A method called by SpriteKit after the reference node’s contents are loaded.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func didLoad(_ node: SKNode?)
```

**watchOS**

``` source
func didLoad(_ node: SKNode?)
```

## Parameters 

`node`  

The deserialized content’s root node.

## Discussion

This method is called after the referenced content is added as a child of the reference node. Override this method in a subclass to implement custom loading behavior.

