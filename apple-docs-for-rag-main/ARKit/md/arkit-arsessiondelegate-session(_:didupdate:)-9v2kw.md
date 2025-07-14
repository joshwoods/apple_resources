

- ARKit
- ARSessionDelegate
-  session(\_:didUpdate:) 

Instance Method

# session(\_:didUpdate:)

Provides a newly captured camera image and accompanying AR information to the delegate.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
optional func session(
    _ session: ARSession,
    didUpdate frame: ARFrame
)
```

## Parameters 

`session`  

The session providing information.

`frame`  

An object containing the new camera image and AR information.

## Mentioned in 

Displaying an AR Experience with Metal

## Discussion

Implement this method if you provide your own display for rendering an AR experience. The provided ARFrame object contains the latest image captured from the device camera, which you can render as a scene background, as well as information about camera parameters and anchor transforms you can use for rendering virtual content on top of the camera image.

