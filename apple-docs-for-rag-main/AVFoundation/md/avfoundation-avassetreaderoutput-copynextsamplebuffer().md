

- AVFoundation
- AVAssetReaderOutput
-  copyNextSampleBuffer() 

Instance Method

# copyNextSampleBuffer()

Copies the next sample buffer from the output.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
func copyNextSampleBuffer() -> CMSampleBuffer?
```

## Return Value

The output sample buffer, or `nil` if you’ve read all samples or an error occurs.

## Discussion

This method returns `nil` when you’ve read all available sample buffers, or if there’s an error. Check the value of the asset reader’s status property to determine the reason.

