

- Core Services
- File System Events
-  FSEventStreamRelease(\_:) 

Function

# FSEventStreamRelease(\_:)

Mac Catalyst 13.1+macOS 10.5+

``` source
func FSEventStreamRelease(_ streamRef: FSEventStreamRef)
```

## Parameters 

`streamRef`  

A valid stream.

## Discussion

Decrements the stream's refcount. The refcount is initially one and is incremented via FSEventStreamRetain(). If the refcount reaches zero then the stream is deallocated.

