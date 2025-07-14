

- RealityKit
-  Contact 

Structure

# Contact

Events associated with collisions.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct Contact
```

## Overview

To subscribe to a collision event, import Combine, create a property of type Cancellable so that you maintain a reference to the subscription, then call subscribe(to:on:_:) or subscribe(to:on:componentType:_:) and provide a closure.

The closure is passed an `RealityKit/Scene/Event` object that contains information relevant to the type of event you subscribed to.

Here’s an example of subscribing to the collision begain event and retrieving the two entities involved in the collision:

```
 import AppKit
 import RealityKit
 import Combine

 class GameViewController: NSViewController {

     @IBOutlet var arView: ARView!
     var collisionSubscription:Cancellable?

     override func awakeFromNib() {
        let boxAnchor = try! Experience.loadBox()
        arView.scene.anchors.append(boxAnchor)

        collisionSubscription = arView.scene.subscribe(
           to: CollisionEvents.Began.self,
            on: boxAnchor
       ) { event in
           print("collision started")
           let firstEntity = event.entityA
           let secondEntity = event.entityB
           // Take appropriate action...
        }
   }
 }
```

You can also create a function to respond to the event rather than a closure by using sink(receiveCompletion:receiveValue:). Here’s an example of using a function to respond to a collision event:

```
import AppKit
import RealityKit
import Combine

class GameViewController: NSViewController {

    @IBOutlet var arView: ARView!
    var collisionSubscription:Cancellable?

    override func awakeFromNib() {
        let boxAnchor = try! Experience.loadBox()
        arView.scene.anchors.append(boxAnchor)

        collisionSubscription = arView.scene.publisher(for: CollisionEvents.Began.self,
                                                       on:nil).sink(receiveValue: onCollisionBegan)
    }

    private func onCollisionBegan(_ event:
                                  CollisionEvents.Began) {
        print("collision started")
        let firstEntity = event.entityA
        let secondEntity = event.entityB
        // Take appropriate action...
    }
}
```

## Topics

### Instance Properties

let impulse: Float

Impulse, the force over time of the collision, in newton-seconds

let impulseDirection: SIMD3&lt;Float>

Impulse direction in scene coordinate space.

let normal: SIMD3&lt;Float>

The normal of the contacting surfaces at the contact point. The normal direction points from the second shape to the first shape in scene coordinate space.

let penetrationDistance: Float

The distance of overlap between the contact pair.

let point: SIMD3&lt;Float>

Point of contact in scene coordinate space.

## Relationships

### Conforms To

- Sendable

## See Also

### Collision-related notifications

enum CollisionEvents

