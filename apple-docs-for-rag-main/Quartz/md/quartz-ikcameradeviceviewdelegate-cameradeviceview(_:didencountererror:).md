

- Quartz
- IKCameraDeviceViewDelegate
-  cameraDeviceView(\_:didEncounterError:) 

Instance Method

# cameraDeviceView(\_:didEncounterError:)

Invoked when the camera encounters an error.

macOS 10.6+

``` source
optional func cameraDeviceView(
    _ cameraDeviceView: IKCameraDeviceView!,
    didEncounterError error: (any Error)!
)
```

## Parameters 

`cameraDeviceView`  

The camera device view that sent the message.

`error`  

The error.

