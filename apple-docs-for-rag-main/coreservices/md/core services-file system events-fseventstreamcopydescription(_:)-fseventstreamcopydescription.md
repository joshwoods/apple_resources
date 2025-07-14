

- Core Services
- File System Events
-  FSEventStreamCopyDescription(\_:) 

Function

# FSEventStreamCopyDescription(\_:)

Mac Catalyst 13.1+macOS 10.5+

``` source
func FSEventStreamCopyDescription(_ streamRef: ConstFSEventStreamRef) -> CFString
```

## Return Value

A CFStringRef containing the description of the supplied stream. Ownership follows the Copy rule.

## Discussion

Returns a CFStringRef containing the description of the supplied stream. For debugging only.

