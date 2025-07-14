

- RoomPlan
- RoomCaptureViewDelegate
-  captureView(didPresent:error:) 

Instance Method

# captureView(didPresent:error:)

Provides the delegate with the post-processed scan results once the view presents them.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 16.0–1.0Deprecated

``` source
func captureView(
    didPresent processedResult: CapturedRoom,
    error: (any Error)?
)
```

## See Also

### Default implementations

func captureView(shouldPresent: CapturedRoomData, error: (any Error)?) -> Bool

Indicates that the app receives and displays post-processed scan results when the scan session stops.

