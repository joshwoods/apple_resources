

- Video Toolbox
-  VTFrameSiloCreate(allocator:fileURL:timeRange:options:frameSiloOut:) 

Function

# VTFrameSiloCreate(allocator:fileURL:timeRange:options:frameSiloOut:)

Creates a frame silo object using a temporary file.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.2+visionOS 1.0+

``` source
func VTFrameSiloCreate(
    allocator: CFAllocator?,
    fileURL: CFURL?,
    timeRange: CMTimeRange,
    options: CFDictionary?,
    frameSiloOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`allocator`  

An allocator for the frame silo. Pass `NULL` to use the default allocator.

`fileURL`  

The URL of the backing file for the `VTFrameSilo` object. If you pass `NULL` for `fileURL`, VideoToolbox will pick a unique temporary file name.

`timeRange`  

The valid time range for the frame silo. Must be valid for progress reporting.

`options`  

Reserved, pass `NULL`.

`frameSiloOut`  

Points to a VTFrameSilo to receive the newly created object. Call `CFRelease` to release your retain on the created VTFrameSilo object when you are done with it.

## Discussion

You can use the returned frame silo object to gather frames produced by multipass encoding.

Call CFRelease to release the frame silo object when you are done with it.

