

- ARKit
- ARSessionDelegate
-  session(\_:didAdd:) 

Instance Method

# session(\_:didAdd:)

Tells the delegate that one or more anchors have been added to the session.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
optional func session(
    _ session: ARSession,
    didAdd anchors: [ARAnchor]
)
```

## Parameters 

`session`  

The session providing information.

`anchors`  

The anchors newly added to the session.

## Discussion

Depending on the session configuration, ARKit may automatically add anchors to a session.

If you display an AR experience using SceneKit or SpriteKit, you can instead implement one of the following methods instead to track not only the addition of anchors to the session but also how to add SceneKit or SpriteKit content to the corresponding scene:

- ARSCNView: renderer(_:nodeFor:) or renderer(_:didAdd:for:)

- ARSKView: node(for:) or view(_:didAdd:for:)

## See Also

### Handling Content Updates

func session(ARSession, didUpdate: [ARAnchor])

Tells the delegate that the session has adjusted the properties of one or more anchors.

func session(ARSession, didRemove: [ARAnchor])

Tells the delegate that one or more anchors have been removed from the session.

