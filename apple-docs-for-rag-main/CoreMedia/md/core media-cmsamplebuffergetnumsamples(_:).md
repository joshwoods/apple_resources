

- Core Media
-  CMSampleBufferGetNumSamples(\_:) 

Function

# CMSampleBufferGetNumSamples(\_:)

Returns the number of media samples in a sample buffer.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSampleBufferGetNumSamples(_ sbuf: CMSampleBuffer) -> CMItemCount
```

## Parameters 

`sbuf`  

The `CMSampleBuffer` being interrogated.

## Return Value

The number of media samples in the `CMSampleBuffer`. 0 is returned if there is an error.

## See Also

### Inspecting Size Information

func CMSampleBufferGetTotalSampleSize(CMSampleBuffer) -> Int

Returns the total size in bytes of sample data in a sample buffer.

func CMSampleBufferGetSampleSize(CMSampleBuffer, at: CMItemIndex) -> Int

Returns the size in bytes of a specified sample in a sample buffer.

func CMSampleBufferGetSampleSizeArray(CMSampleBuffer, entryCount: CMItemCount, arrayToFill: UnsafeMutablePointer&lt;Int>?, entriesNeededOut: UnsafeMutablePointer&lt;CMItemCount>?) -> OSStatus

Retrieves an array of sample sizes that represents each sample in a sample buffer.

