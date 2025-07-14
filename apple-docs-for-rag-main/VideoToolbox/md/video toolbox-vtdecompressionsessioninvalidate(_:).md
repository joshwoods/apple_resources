

- Video Toolbox
-  VTDecompressionSessionInvalidate(\_:) 

Function

# VTDecompressionSessionInvalidate(\_:)

Tears down a decompression session.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
func VTDecompressionSessionInvalidate(_ session: VTDecompressionSession)
```

## Parameters 

`session`  

The decompression session to invalidate.

## Discussion

When you finish with a decompression session you created, call this function to tear it down, and then CFRelease to release your object reference.

Note

A decompression session is automatically invalidated when its retain count reaches zero, but because sessions may be retained by multiple parties, it can be hard to predict when this will happen. Calling `VTDecompressionSessionInvalidate` ensures a deterministic, orderly teardown.

