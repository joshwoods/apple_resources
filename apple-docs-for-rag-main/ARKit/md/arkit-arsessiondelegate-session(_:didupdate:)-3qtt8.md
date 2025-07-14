

- ARKit
- ARSessionDelegate
-  session(\_:didUpdate:) 

Instance Method

# session(\_:didUpdate:)

Tells the delegate that the session has adjusted the properties of one or more anchors.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
optional func session(
    _ session: ARSession,
    didUpdate anchors: [ARAnchor]
)
```

## Parameters 

`session`  

The session providing information.

`anchors`  

The anchors whose properties have changed.

## Discussion

Depending on the session configuration, ARKit may automatically update the properties of anchors in a session.

If you display an AR experience using SceneKit or SpriteKit, you can implement one of the following methods instead to track not only the anchors in the session but also any corresponding SceneKit or SpriteKit content:

- ARSCNView: renderer(_:willUpdate:for:) or renderer(_:didUpdate:for:)

- ARSKView: view(_:willUpdate:for:) or view(_:didUpdate:for:)

## See Also

### Handling Content Updates

func session(ARSession, didAdd: [ARAnchor])

Tells the delegate that one or more anchors have been added to the session.

func session(ARSession, didRemove: [ARAnchor])

Tells the delegate that one or more anchors have been removed from the session.

