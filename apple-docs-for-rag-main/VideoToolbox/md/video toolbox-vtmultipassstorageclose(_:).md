

- Video Toolbox
-  VTMultiPassStorageClose(\_:) 

Function

# VTMultiPassStorageClose(\_:)

Ensures that any pending data is written to the multipass storage file and closes the file.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.2+visionOS 1.0+

``` source
func VTMultiPassStorageClose(_ multiPassStorage: VTMultiPassStorage) -> OSStatus
```

## Parameters 

`multiPassStorage`  

The multipass storage object to close.

## Discussion

After this function is called, all functions on the multipass storage object fail. It’s still necessary to release the object by calling CFRelease.

