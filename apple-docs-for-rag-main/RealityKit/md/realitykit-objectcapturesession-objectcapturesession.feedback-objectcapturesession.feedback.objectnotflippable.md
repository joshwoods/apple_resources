

- RealityKit
- ObjectCaptureSession
- ObjectCaptureSession.Feedback
-  ObjectCaptureSession.Feedback.objectNotFlippable 

Case

# ObjectCaptureSession.Feedback.objectNotFlippable

It is not recommended to flip this object since is is unlikely the algorithm will be able to stitch the flipped orientation. This is usually due to feature-less, low-texture objects. In this case, multiple passes at different heights leaving object at its original orientation are recommended instead of flipping.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+

``` source
case objectNotFlippable
```

