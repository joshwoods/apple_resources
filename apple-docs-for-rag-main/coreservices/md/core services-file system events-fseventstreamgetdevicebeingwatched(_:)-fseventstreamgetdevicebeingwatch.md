

- Core Services
- File System Events
-  FSEventStreamGetDeviceBeingWatched(\_:) 

Function

# FSEventStreamGetDeviceBeingWatched(\_:)

Mac Catalyst 13.1+macOS 10.5+

``` source
func FSEventStreamGetDeviceBeingWatched(_ streamRef: ConstFSEventStreamRef) -> dev_t
```

## Parameters 

`streamRef`  

A valid stream.

## Return Value

The dev_t for a device-relative stream, otherwise 0.

## Discussion

Fetches the dev_t supplied when the stream was created via FSEventStreamCreateRelativeToDevice(), otherwise 0.

