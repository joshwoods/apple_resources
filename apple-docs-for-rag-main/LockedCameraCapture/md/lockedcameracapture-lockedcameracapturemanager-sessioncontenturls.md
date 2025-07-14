

- LockedCameraCapture
- LockedCameraCaptureManager
-  sessionContentURLs 

Instance Property

# sessionContentURLs

An array of URLs that each point to a directory containing captured content.

iOS 18.0+iPadOS 18.0+

``` source
final var sessionContentURLs: [URL] { get }
```

## Discussion

Content in the URLs is captured during a capture extension’s LockedCameraCaptureSession. These directories are located within the capture extension’s containing app’s data container.

