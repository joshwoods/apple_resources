

- AppKit
- NSWorkspace
- NSWorkspace.AuthorizationType
-  NSWorkspace.AuthorizationType.replaceFile 

Case

# NSWorkspace.AuthorizationType.replaceFile

Authorization for the app to perform an atomic file write without changing the target file’s permissions.

macOS 10.14+

``` source
case replaceFile
```

## Discussion

Signifies that the user has granted authorization for replaceItem(at:withItemAt:backupItemName:options:resultingItemURL:). When you use a FileManager with this authorization, the file manager ignores the `backupItemName` and `options` parameters.

## See Also

### Types of Authorization

case createSymbolicLink

Authorization for the app to create a symbolic link.

case setAttributes

Authorization for the app to change specific file attributes.

