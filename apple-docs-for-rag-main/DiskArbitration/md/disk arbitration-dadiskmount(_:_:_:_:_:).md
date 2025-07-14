

- Disk Arbitration
-  DADiskMount(\_:\_:\_:\_:\_:) 

Function

# DADiskMount(\_:\_:\_:\_:\_:)

Mounts the volume at the specified disk object.

Mac Catalyst 13.1+macOS 10.4+

``` source
func DADiskMount(
    _ disk: DADisk,
    _ path: CFURL?,
    _ options: DADiskMountOptions,
    _ callback: DADiskMountCallback?,
    _ context: UnsafeMutableRawPointer?
)
```

## Parameters 

`disk`  

The disk object.

`path`  

The mount path. Pass NULL for a “standard” mount path.

`options`  

The mount options.

`callback`  

The callback function to call once the mount completes.

`context`  

The user-defined context parameter to pass to the callback function.

## See Also

### Miscellaneous

func DADiskClaim(DADisk, DADiskClaimOptions, DADiskClaimReleaseCallback?, UnsafeMutableRawPointer?, DADiskClaimCallback?, UnsafeMutableRawPointer?)

Claims the specified disk object for exclusive use.

func DADiskEject(DADisk, DADiskEjectOptions, DADiskEjectCallback?, UnsafeMutableRawPointer?)

Ejects the specified disk object.

func DADiskGetOptions(DADisk) -> DADiskOptions

Obtains the options for the specified disk.

func DADiskIsClaimed(DADisk) -> Bool

Reports whether or not the disk is claimed.

func DADiskMountWithArguments(DADisk, CFURL?, DADiskMountOptions, DADiskMountCallback?, UnsafeMutableRawPointer?, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>?)

Mounts the volume at the specified disk object, with the specified mount options.

func DADiskRename(DADisk, CFString, DADiskRenameOptions, DADiskRenameCallback?, UnsafeMutableRawPointer?)

Renames the volume at the specified disk object.

func DADiskSetOptions(DADisk, DADiskOptions, Bool) -> DAReturn

Sets the options for the specified disk.

func DADiskUnclaim(DADisk)

Unclaims the specified disk object.

func DADiskUnmount(DADisk, DADiskUnmountOptions, DADiskUnmountCallback?, UnsafeMutableRawPointer?)

Unmounts the volume at the specified disk object.

func DARegisterDiskAppearedCallback(DASession, CFDictionary?, DADiskAppearedCallback, UnsafeMutableRawPointer?)

Registers a callback function to be called whenever a disk has appeared.

func DARegisterDiskDescriptionChangedCallback(DASession, CFDictionary?, CFArray?, DADiskDescriptionChangedCallback, UnsafeMutableRawPointer?)

Registers a callback function to be called whenever a disk description has changed.

func DARegisterDiskDisappearedCallback(DASession, CFDictionary?, DADiskDisappearedCallback, UnsafeMutableRawPointer?)

Registers a callback function to be called whenever a disk has disappeared.

func DARegisterDiskEjectApprovalCallback(DASession, CFDictionary?, DADiskEjectApprovalCallback, UnsafeMutableRawPointer?)

Registers a callback function to be called whenever a volume is to be ejected.

func DARegisterDiskMountApprovalCallback(DASession, CFDictionary?, DADiskMountApprovalCallback, UnsafeMutableRawPointer?)

Registers a callback function to be called whenever a volume is to be mounted.

func DARegisterDiskPeekCallback(DASession, CFDictionary?, CFIndex, DADiskPeekCallback, UnsafeMutableRawPointer?)

Registers a callback function to be called whenever a disk has been probed.

