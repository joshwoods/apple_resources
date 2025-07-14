

- Core Services
- Carbon Core
- Carbon Core Functions
-  LSSharedFileListInsertItemURL(\_:\_:\_:\_:\_:\_:\_:) Deprecated

Function

# LSSharedFileListInsertItemURL(\_:\_:\_:\_:\_:\_:\_:)

macOS 10.5–10.11Deprecated

``` source
func LSSharedFileListInsertItemURL(
    _ inList: LSSharedFileList,
    _ insertAfterThisItem: LSSharedFileListItem,
    _ inDisplayName: CFString?,
    _ inIconRef: IconRef?,
    _ inURL: CFURL,
    _ inPropertiesToSet: CFDictionary?,
    _ inPropertiesToClear: CFArray?
) -> LSSharedFileListItem?
```

