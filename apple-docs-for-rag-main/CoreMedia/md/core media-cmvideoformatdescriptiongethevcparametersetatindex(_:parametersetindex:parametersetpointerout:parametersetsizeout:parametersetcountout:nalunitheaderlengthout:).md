

- Core Media
-  CMVideoFormatDescriptionGetHEVCParameterSetAtIndex(\_:parameterSetIndex:parameterSetPointerOut:parameterSetSizeOut:parameterSetCountOut:nalUnitHeaderLengthOut:) 

Function

# CMVideoFormatDescriptionGetHEVCParameterSetAtIndex(\_:parameterSetIndex:parameterSetPointerOut:parameterSetSizeOut:parameterSetCountOut:nalUnitHeaderLengthOut:)

Returns a parameter set contained in an HEVC (H.265) format description.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 6.0+

``` source
func CMVideoFormatDescriptionGetHEVCParameterSetAtIndex(
    _ videoDesc: CMFormatDescription,
    parameterSetIndex: Int,
    parameterSetPointerOut: UnsafeMutablePointer?>?,
    parameterSetSizeOut: UnsafeMutablePointer?,
    parameterSetCountOut: UnsafeMutablePointer?,
    nalUnitHeaderLengthOut NALUnitHeaderLengthOut: UnsafeMutablePointer?
) -> OSStatus
```

## See Also

### Functions

func CMTimeFoldIntoRange(CMTime, foldRange: CMTimeRange) -> CMTime

Folds a time into a time range.

