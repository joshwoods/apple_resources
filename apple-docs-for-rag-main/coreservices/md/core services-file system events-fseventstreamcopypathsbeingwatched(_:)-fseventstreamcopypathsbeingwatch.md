

- Core Services
- File System Events
-  FSEventStreamCopyPathsBeingWatched(\_:) 

Function

# FSEventStreamCopyPathsBeingWatched(\_:)

Mac Catalyst 13.1+macOS 10.5+

``` source
func FSEventStreamCopyPathsBeingWatched(_ streamRef: ConstFSEventStreamRef) -> CFArray
```

## Parameters 

`streamRef`  

A valid stream.

## Return Value

A CFArray of CFStringRefs corresponding to those supplied when the stream was created. Ownership follows the Copy rule.

## Discussion

Fetches the paths supplied when the stream was created via one of the FSEventStreamCreate...() functions.

