

- AppKit
- NSWorkspace
- NSWorkspace.AuthorizationType
-  NSWorkspace.AuthorizationType.createSymbolicLink 

Case

# NSWorkspace.AuthorizationType.createSymbolicLink

Authorization for the app to create a symbolic link.

macOS 10.14+

``` source
case createSymbolicLink
```

## Discussion

Signifies that the user has granted authorization for createSymbolicLink(at:withDestinationURL:).

## See Also

### Types of Authorization

case replaceFile

Authorization for the app to perform an atomic file write without changing the target file’s permissions.

case setAttributes

Authorization for the app to change specific file attributes.

