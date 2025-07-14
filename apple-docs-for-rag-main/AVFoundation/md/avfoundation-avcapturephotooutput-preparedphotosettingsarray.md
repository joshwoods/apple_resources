

- AVFoundation
- AVCapturePhotoOutput
-  preparedPhotoSettingsArray 

Instance Property

# preparedPhotoSettingsArray

An array of photo settings for which the photo output has prepared capture resources.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var preparedPhotoSettingsArray: [AVCapturePhotoSettings] { get }
```

## Discussion

Some types of photo capture, such as bracketed captures and RAW captures, require the photo output to allocate additional buffers or prepare other resources. To prevent photo capture requests from executing slowly due to lazy resource allocation, you may call the setPreparedPhotoSettingsArray(_:completionHandler:) method with an array of settings objects representative of the types of capture you will be performing (such as settings for a bracketed capture, RAW capture, or capture with still image stabilization).

By default, the photo output prepares sufficient resources to capture photos with default settings (as defined by the AVCapturePhotoSettings default initializer).

## See Also

### Preparing for Resource-Intensive Captures

func setPreparedPhotoSettingsArray([AVCapturePhotoSettings], completionHandler: ((Bool, (any Error)?) -> Void)?)

Tells the photo capture output to prepare resources for future capture requests with the specified settings.

