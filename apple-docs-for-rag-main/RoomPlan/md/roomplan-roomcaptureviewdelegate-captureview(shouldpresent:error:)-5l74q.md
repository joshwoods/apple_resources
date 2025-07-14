

- RoomPlan
- RoomCaptureViewDelegate
-  captureView(shouldPresent:error:) 

Instance Method

# captureView(shouldPresent:error:)

Indicates that the app receives and displays post-processed scan results when the scan session stops.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 16.0–1.0Deprecated

``` source
func captureView(
    shouldPresent roomDataForProcessing: CapturedRoomData,
    error: (any Error)?
) -> Bool
```

## Parameters 

`roomDataForProcessing`  

A data object that contains the raw scan results.

`error`  

An object that describes the problem when an error occurs; otherwise, `nil`.

## Return Value

This implementation always returns `true`.

## Discussion

If your app’s room-capture view delegate doesn’t implement captureView(shouldPresent:error:), then the framework calls this default implementation.

## See Also

### Default implementations

func captureView(didPresent: CapturedRoom, error: (any Error)?)

Provides the delegate with the post-processed scan results once the view presents them.

