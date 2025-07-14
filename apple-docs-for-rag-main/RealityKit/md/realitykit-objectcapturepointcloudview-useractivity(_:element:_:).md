

- RealityKit
- ObjectCapturePointCloudView
-  userActivity(\_:element:\_:) 

Instance Method

# userActivity(\_:element:\_:)

Advertises a user activity type.

RealityKitSwiftUIiOS 14.0+iPadOS 14.0+macOS 11.0+tvOS 14.0+watchOS 7.0+

``` source
nonisolated
func userActivity(
    _ activityType: String,
    element: P?,
    _ update: @escaping (P, NSUserActivity) -> ()
) -> some View
```

## Parameters 

`activityType`  

The type of activity to advertise.

`element`  

If the element is `nil`, the handler will not be associated with the activity (and if there are no handlers, no activity is advertised). The method passes the non-`nil` element to the handler as a convenience so the handlers don’t all need to implement an early exit with `guard element = element else { return }`.

`update`  

A function that modifies the passed-in activity for advertisement.

## Discussion

The scope of the activity applies only to the scene or window the view is in.

