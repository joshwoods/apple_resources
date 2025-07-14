

- LockedCameraCapture
- LockedCameraCaptureManager
-  sessionContentUpdates 

Instance Property

# sessionContentUpdates

An `AsyncSequence` to process captured content from your capture extension.

iOS 18.0+iPadOS 18.0+

``` source
final var sessionContentUpdates: some AsyncSequence { get }
```

## Discussion

Use this to process captured content as soon as it is available after your app launches.

