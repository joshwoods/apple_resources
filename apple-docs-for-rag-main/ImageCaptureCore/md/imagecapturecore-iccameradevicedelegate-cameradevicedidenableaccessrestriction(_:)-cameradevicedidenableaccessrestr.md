

- ImageCaptureCore
- ICCameraDeviceDelegate
-  cameraDeviceDidEnableAccessRestriction(\_:) 

Instance Method

# cameraDeviceDidEnableAccessRestriction(\_:)

Tells the client when an Apple device has been locked, and media is unavailable until the restriction has been removed.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+

``` source
func cameraDeviceDidEnableAccessRestriction(_ device: ICDevice)
```

**Required**

## See Also

### Responding to Access Restrictions

func cameraDeviceDidRemoveAccessRestriction(ICDevice)

Tells the client when an Apple device has been unlocked, paired to the host, and media is available.

**Required**

