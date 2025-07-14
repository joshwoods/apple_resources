

- RealityKit
- ObjectCaptureView
-  hideObjectReticle(\_:) 

Instance Method

# hideObjectReticle(\_:)

Hides the object selection reticle when the session is in `.ready` state if set to true. Example: ObjectCaptureView(session: mySession) .hideObjectReticle()

RealityKitSwiftUIiOS 18.0+iPadOS 18.0+

``` source
@MainActor @preconcurrency
func hideObjectReticle(_ value: Bool = true) -> ObjectCaptureView
```

Available when `Overlay` conforms to `View`.

## Discussion

It can also be passed a value if there is a state variable controlling it:

ObjectCaptureView(session: mySession) .hideObjectReticle(shouldHideObjectReticle)

Other modifiers can be chained to build the final view: ObjectCaptureView(session: mySession) .hideObjectReticle() .transition(.opacity)

