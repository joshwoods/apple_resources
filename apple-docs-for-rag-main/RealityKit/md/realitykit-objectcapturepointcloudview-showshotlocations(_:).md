

- RealityKit
- ObjectCapturePointCloudView
-  showShotLocations(\_:) 

Instance Method

# showShotLocations(\_:)

Shows the locations where shots have been taken. Example: ObjectCapturePointCloudView(session: mySession) .showShotLocations()

RealityKitSwiftUIiOS 18.0+iPadOS 18.0+

``` source
@MainActor
func showShotLocations(_ value: Bool = true) -> ObjectCapturePointCloudView
```

## Discussion

It can also be passed a value if there is a state variable controlling it:

ObjectCapturePointCloudView(session: mySession) .showShotLocations(shouldShowShots)

Other modifiers can be chained to build the final view: ObjectCapturePointCloudView(session: mySession) .showShotLocations() .transition(.opacity)

