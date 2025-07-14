

- LockedCameraCapture
- LockedCameraCaptureManager
-  LockedCameraCaptureManager.SessionContentUpdate 

Enumeration

# LockedCameraCaptureManager.SessionContentUpdate

URLs provided by the sessionContentUpdates `AsyncSequence`.

iOS 18.0+iPadOS 18.0+

``` source
enum SessionContentUpdate
```

## Topics

### Enumeration Cases

case added(url: URL)

A URL to a directory of added session content.

case initial(urls: [URL])

URLs to directories of the current session content available when beginning observation of sessionContentUpdates.

case removed(url: URL)

A URL to a directory of removed session content.

## Relationships

### Conforms To

- Sendable

