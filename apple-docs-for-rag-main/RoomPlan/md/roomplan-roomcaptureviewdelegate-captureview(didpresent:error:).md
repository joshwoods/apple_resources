

- RoomPlan
- RoomCaptureViewDelegate
-  captureView(didPresent:error:) 

Instance Method

# captureView(didPresent:error:)

Provides the delegate with the processed scan results as the view presents them.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 16.0–1.0Deprecated

``` source
func captureView(
    didPresent processedResult: CapturedRoom,
    error: (any Error)?
)
```

**Required** Default implementation provided.

## Parameters 

`processedResult`  

A structure that provides detailed information about the dimensions and features of the scanned room.

`error`  

An object that describes the problem when an error occurs; otherwise, `nil`.

## Discussion

The framework invokes this callback when your app returns `true` for captureView(shouldPresent:error:).

With the `processedResult` argument, your app can alter the detailed captured room object or export it to a USDZ file.

## Default Implementations

### RoomCaptureViewDelegate Implementations

func captureView(didPresent: CapturedRoom, error: (any Error)?)

Provides the delegate with the post-processed scan results once the view presents them.

## See Also

### Post-processing scan results

func captureView(shouldPresent: CapturedRoomData, error: (any Error)?) -> Bool

Indicates whether the app processes raw scan results immediately after a scan session stops.

**Required** Default implementation provided.

