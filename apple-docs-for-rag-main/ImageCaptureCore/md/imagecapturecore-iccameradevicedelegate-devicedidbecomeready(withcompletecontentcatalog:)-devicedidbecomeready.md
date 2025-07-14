

- ImageCaptureCore
- ICCameraDeviceDelegate
-  deviceDidBecomeReady(withCompleteContentCatalog:) 

Instance Method

# deviceDidBecomeReady(withCompleteContentCatalog:)

Tells the client that the camera device is done enumerating its content and is ready to receive requests.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
func deviceDidBecomeReady(withCompleteContentCatalog device: ICCameraDevice)
```

**Required**

## Discussion

You must open a session on the device before you can enumerate its content and make it ready to receive requests.

