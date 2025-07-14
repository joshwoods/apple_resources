

- Core Services
- Carbon Core
- Carbon Core Functions
-  LSSharedFileListInsertItemFSRef(\_:\_:\_:\_:\_:\_:\_:) Deprecated

Function

# LSSharedFileListInsertItemFSRef(\_:\_:\_:\_:\_:\_:\_:)

macOS 10.5–10.10Deprecated

``` source
func LSSharedFileListInsertItemFSRef(
    _ inList: LSSharedFileList,
    _ insertAfterThisItem: LSSharedFileListItem,
    _ inDisplayName: CFString?,
    _ inIconRef: IconRef?,
    _ inFSRef: UnsafePointer,
    _ inPropertiesToSet: CFDictionary?,
    _ inPropertiesToClear: CFArray?
) -> LSSharedFileListItem?
```

