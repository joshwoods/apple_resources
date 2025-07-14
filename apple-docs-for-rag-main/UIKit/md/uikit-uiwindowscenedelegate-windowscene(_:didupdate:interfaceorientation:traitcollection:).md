

- UIKit
- UIWindowSceneDelegate
-  windowScene(\_:didUpdate:interfaceOrientation:traitCollection:) 

Instance Method

# windowScene(\_:didUpdate:interfaceOrientation:traitCollection:)

Notifies you when the size, orientation, or traits of a scene change.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func windowScene(
    _ windowScene: UIWindowScene,
    didUpdate previousCoordinateSpace: any UICoordinateSpace,
    interfaceOrientation previousInterfaceOrientation: UIInterfaceOrientation,
    traitCollection previousTraitCollection: UITraitCollection
)
```

## Parameters 

`windowScene`  

The window scene object whose environment changed.

`previousCoordinateSpace`  

The previous coordinate space of the scene. Get the current coordinate space from the coordinateSpace property of the `windowScene` object.

`previousInterfaceOrientation`  

The previous interface orientation for your content. Get the current interface orientation from the interfaceOrientation property of the `windowScene` object.

`previousTraitCollection`  

The previous traits for the window. Get the current window traits from the traitCollection property of the `windowScene` object.

## Mentioned in 

Presenting content on a connected display

## Discussion

The window scene environment typically changes in response to user actions. For example, the interface orientation changes in response to device orientation changes or screen mode in response to moving to another screen. Similarly, the user may resize scenes on iPad, which causes UIKit to report a change to the scene’s coordinate space. Use these changes to make any needed changes to your scene’s content or interface.

## See Also

### Related Documentation

Presenting content on a connected display

Fill connected displays with additional content from your app.

