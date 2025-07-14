

- WatchKit
- WKInterfaceHMCamera
-  setCameraSource(\_:) 

Instance Method

# setCameraSource(\_:)

Set the HomeKit camera source displayed by this interface object.

watchOS 3.0+

``` source
func setCameraSource(_ cameraSource: HMCameraSource?)
```

## Parameters 

`cameraSource`  

A HomeKit camera source, representing a video stream or a single snapshot from an IP camera.

## Discussion

Pass `nil` to clear the camera source.

