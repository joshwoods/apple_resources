

- Video Toolbox
-  VTMultiPassStorageCreate(allocator:fileURL:timeRange:options:multiPassStorageOut:) 

Function

# VTMultiPassStorageCreate(allocator:fileURL:timeRange:options:multiPassStorageOut:)

Creates a multipass storage object using a temporary file.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.2+visionOS 1.0+

``` source
func VTMultiPassStorageCreate(
    allocator: CFAllocator?,
    fileURL: CFURL?,
    timeRange: CMTimeRange,
    options: CFDictionary?,
    multiPassStorageOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`allocator`  

An allocator for the session. Pass `NULL` to use the default allocator.

`fileURL`  

Specifies where to put the backing file for the multipass storage object. If you pass `NULL` for `fileURL`, the video toolbox will pick a unique temporary file name.

`timeRange`  

Gives a hint to the multipass storage about valid time stamps for data. You can pass `kCMTimeRangeInvalid` if you do not want to provide a time range hint.

`options`  

If the file did not exist when the storage was created, the file will be deleted when the multipass storage object is finalized, unless you set the kVTMultiPassStorageCreationOption_DoNotDelete option to kCFBooleanTrue in the `options` dictionary.

`multiPassStorageOut`  

A pointer to the newly created multipass storage object.

## Discussion

You can use the multipass storage object to perform multipass encoding; see kVTCompressionPropertyKey_MultiPassStorage.

Call CFRelease to release the multipass storage object when you are done with it.

