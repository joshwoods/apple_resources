

- Core Media
-  CMTimeFoldIntoRange(\_:foldRange:) 

Function

# CMTimeFoldIntoRange(\_:foldRange:)

Folds a time into a time range.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTimeFoldIntoRange(
    _ time: CMTime,
    foldRange: CMTimeRange
) -> CMTime
```

## Parameters 

`time`  

The time to fold.

`foldRange`  

The time range into which to fold the time.

## Return Value

A time that represents the translated duration.

## See Also

### Functions

func CMVideoFormatDescriptionGetHEVCParameterSetAtIndex(CMFormatDescription, parameterSetIndex: Int, parameterSetPointerOut: UnsafeMutablePointer&lt;UnsafePointer&lt;UInt8>?>?, parameterSetSizeOut: UnsafeMutablePointer&lt;Int>?, parameterSetCountOut: UnsafeMutablePointer&lt;Int>?, nalUnitHeaderLengthOut: UnsafeMutablePointer&lt;Int32>?) -> OSStatus

Returns a parameter set contained in an HEVC (H.265) format description.

