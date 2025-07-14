

- ImageCaptureCore
- ICCameraDeviceDelegate
-  cameraDeviceDidRemoveAccessRestriction(\_:) 

Instance Method

# cameraDeviceDidRemoveAccessRestriction(\_:)

Tells the client when an Apple device has been unlocked, paired to the host, and media is available.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+

``` source
func cameraDeviceDidRemoveAccessRestriction(_ device: ICDevice)
```

**Required**

## See Also

### Responding to Access Restrictions

func cameraDeviceDidEnableAccessRestriction(ICDevice)

Tells the client when an Apple device has been locked, and media is unavailable until the restriction has been removed.

**Required**

