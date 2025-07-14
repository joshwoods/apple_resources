

- ARKit
- ARSessionDelegate
-  session(\_:didRemove:) 

Instance Method

# session(\_:didRemove:)

Tells the delegate that one or more anchors have been removed from the session.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
optional func session(
    _ session: ARSession,
    didRemove anchors: [ARAnchor]
)
```

## Parameters 

`session`  

The session providing information.

`anchors`  

The anchors newly removed from the session.

## Discussion

Depending on the session configuration, ARKit may automatically remove anchors from a session.

If you display an AR experience using SceneKit or SpriteKit, you can instead implement one of the following methods instead to track not only the anchors in the session but also any corresponding SceneKit or SpriteKit content:

- ARSCNView: renderer(_:didRemove:for:)

- ARSKView: view(_:didRemove:for:)

## See Also

### Handling Content Updates

func session(ARSession, didAdd: [ARAnchor])

Tells the delegate that one or more anchors have been added to the session.

func session(ARSession, didUpdate: [ARAnchor])

Tells the delegate that the session has adjusted the properties of one or more anchors.

