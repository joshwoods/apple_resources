

- AVFoundation
- AVAssetReader
-  startReading() 

Instance Method

# startReading()

Prepares the asset reader to start reading sample buffers from the asset.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
func startReading() -> Bool
```

## Return Value

true if the reader is able to start reading; otherwise, false.

## Discussion

If this method returns false, you can determine the reason by checking the values of the status and error properties.

## See Also

### Controlling Reading

func cancelReading()

Cancels any background work and stops the reader’s outputs from reading more samples.

