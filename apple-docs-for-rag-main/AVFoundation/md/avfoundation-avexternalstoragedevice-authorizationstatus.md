

- AVFoundation
- AVExternalStorageDevice
-  authorizationStatus 

Type Property

# authorizationStatus

Your app’s authorization status for the external storage device.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+

``` source
class var authorizationStatus: AVAuthorizationStatus { get }
```

## Discussion

If the value is AVAuthorizationStatus.notDetermined, you can request access by calling the requestAccess(completionHandler:) method.

