

- AppKit
- NSWorkspace
-  noteFileSystemChanged(\_:) 

Instance Method

# noteFileSystemChanged(\_:)

Informs the workspace object that the file system changed at the specified path.

macOS

``` source
func noteFileSystemChanged(_ path: String)
```

## Parameters 

`path`  

The full path that changed.

## Discussion

Avoid calling this method if possible. If you want to track changes to files and directories, use the FSEvents API described in `FSEvents`.

The NSWorkspace object uses this method to track changes to all the files and directories in which it is interested.

