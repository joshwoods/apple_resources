

- Core Media
-  CMSampleBufferGetFormatDescription(\_:) 

Function

# CMSampleBufferGetFormatDescription(\_:)

Returns the format description of the samples in a sample buffer.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMSampleBufferGetFormatDescription(_ sbuf: CMSampleBuffer) -> CMFormatDescription?
```

## Parameters 

`sbuf`  

The `CMSampleBuffer` being interrogated.

## Return Value

The format description of the samples in the `CMSampleBuffer` or `NULL` if there is an error.

## Discussion

On return, the caller doesn’t own the returned `formatDesc`, and must retain it explicitly if the caller needs to maintain a reference to it.

