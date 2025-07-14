

- Core Services
- Carbon Core
- Carbon Core Functions
-  LSSharedFileListAddObserver(\_:\_:\_:\_:\_:) Deprecated

Function

# LSSharedFileListAddObserver(\_:\_:\_:\_:\_:)

macOS 10.5–10.11Deprecated

``` source
func LSSharedFileListAddObserver(
    _ inList: LSSharedFileList?,
    _ inRunloop: CFRunLoop,
    _ inRunloopMode: CFString,
    _ callback: LSSharedFileListChangedProcPtr,
    _ context: UnsafeMutableRawPointer?
)
```

