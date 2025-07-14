

- LockedCameraCapture
- LockedCameraCaptureManager
-  invalidateSessionContent(at:) 

Instance Method

# invalidateSessionContent(at:)

Tells the system that the app no longer needs the directory at the URL and it can be deleted.

iOS 18.0+iPadOS 18.0+

``` source
final func invalidateSessionContent(at url: URL) async throws
```

## Parameters 

`url`  

A URL from sessionContentURLs. The system ignores other URLs.

## Discussion

The directory at the `URL` contains captured content for a session. Store the captured content appropriately before calling this method, otherwise the system deletes it.

