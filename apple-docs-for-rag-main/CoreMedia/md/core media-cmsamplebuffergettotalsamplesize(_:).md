

- Core Media
-  CMSampleBufferGetTotalSampleSize(\_:) 

Function

# CMSampleBufferGetTotalSampleSize(\_:)

Returns the total size in bytes of sample data in a sample buffer.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSampleBufferGetTotalSampleSize(_ sbuf: CMSampleBuffer) -> Int
```

## Parameters 

`sbuf`  

The `CMSampleBuffer` being interrogated.

## Return Value

Total size in bytes of sample data in the `CMSampleBuffer`. If there are no sample sizes in this `CMSampleBuffer`, a size of 0 will be returned.

## See Also

### Inspecting Size Information

func CMSampleBufferGetNumSamples(CMSampleBuffer) -> CMItemCount

Returns the number of media samples in a sample buffer.

func CMSampleBufferGetSampleSize(CMSampleBuffer, at: CMItemIndex) -> Int

Returns the size in bytes of a specified sample in a sample buffer.

func CMSampleBufferGetSampleSizeArray(CMSampleBuffer, entryCount: CMItemCount, arrayToFill: UnsafeMutablePointer&lt;Int>?, entriesNeededOut: UnsafeMutablePointer&lt;CMItemCount>?) -> OSStatus

Retrieves an array of sample sizes that represents each sample in a sample buffer.

