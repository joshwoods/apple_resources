

- System
- FilePermissions
-  saveText 

Type Property

# saveText

Indicates that executable’s text segment should be kept in swap space even after it exits.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var saveText: FilePermissions { get }
```

## Discussion

For more information, see the `chmod(2)` man page’s discussion of `S_ISVTX` (the sticky bit).

## See Also

### Special Permissions

static var setUserID: FilePermissions

Indicates that the file is executed as the owner.

static var setGroupID: FilePermissions

Indicates that the file is executed as the group.

