

- AppKit
- NSWorkspace
- NSWorkspace.AuthorizationType
-  NSWorkspace.AuthorizationType.setAttributes 

Case

# NSWorkspace.AuthorizationType.setAttributes

Authorization for the app to change specific file attributes.

macOS 10.14+

``` source
case setAttributes
```

## Discussion

Signifies that the user has granted authorization for setAttributes(_:ofItemAtPath:).

Only these attributes can be modified:

- ownerAccountID

- groupOwnerAccountID

- posixPermissions

## See Also

### Types of Authorization

case createSymbolicLink

Authorization for the app to create a symbolic link.

case replaceFile

Authorization for the app to perform an atomic file write without changing the target file’s permissions.

