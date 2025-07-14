

- AVFoundation
- AVAssetReader
-  cancelReading() 

Instance Method

# cancelReading()

Cancels any background work and stops the reader’s outputs from reading more samples.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
func cancelReading()
```

## Discussion

To stop reading samples before reaching the end of the time range, call this method to stop any in-progress background read operations.

## See Also

### Controlling Reading

func startReading() -> Bool

Prepares the asset reader to start reading sample buffers from the asset.

