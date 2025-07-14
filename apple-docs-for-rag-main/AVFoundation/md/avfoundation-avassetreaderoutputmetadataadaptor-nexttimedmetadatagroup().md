

- AVFoundation
- AVAssetReaderOutputMetadataAdaptor
-  nextTimedMetadataGroup() 

Instance Method

# nextTimedMetadataGroup()

Returns the next timed metadata group for the asset reader output.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
func nextTimedMetadataGroup() -> AVTimedMetadataGroup?
```

## Return Value

A timed metadata group that represents the next logical segment of metadata from the source asset reader output.

## Discussion

This method returns `nil` after the adaptor reads all timed metadata groups from the output, or if an error occurs. When the return value is `nil`, check the asset reader’s status property to determine why it couldn’t read more samples.

