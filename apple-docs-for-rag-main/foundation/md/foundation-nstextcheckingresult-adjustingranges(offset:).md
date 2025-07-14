

- Foundation
- NSTextCheckingResult
-  adjustingRanges(offset:) 

Instance Method

# adjustingRanges(offset:)

Returns a new text checking result after adjusting the ranges as specified by the offset.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func adjustingRanges(offset: Int) -> NSTextCheckingResult
```

## Parameters 

`offset`  

The amount the ranges are adjusted.

## Return Value

A new `NSTextCheckingResult` instance with the adjusted range or ranges.

