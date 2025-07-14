

- ARKit
- ARSession
-  delegate 

Instance Property

# delegate

An object you provide to receive captured video images and tracking information, or to respond to changes in session status.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
weak var delegate: (any ARSessionDelegate)? { get set }
```

## Discussion

If you use the ARSCNView or ARSKView class to display your AR experience, a session delegate isn’t necessary. Those views automatically display captured video images and coordinate SceneKit or SpriteKit content to track device and camera motion.

If you create your own visualization for an AR experience using Metal or other rendering technologies, set a session delegate. Your delegate object periodically receives ARFrame objects captured by the session. These objects contain video frame images for you to display and AR scene information you can use to coordinate display of the scene elements you render.

## See Also

### Responding to events

var delegateQueue: dispatch_queue_t?

The dispatch queue through which the session calls your delegate methods.

protocol ARSessionDelegate

Methods you can implement to receive captured video frame images and tracking state from an AR session.

protocol ARSessionObserver

Methods you can implement to respond to changes in the state of an AR session.

