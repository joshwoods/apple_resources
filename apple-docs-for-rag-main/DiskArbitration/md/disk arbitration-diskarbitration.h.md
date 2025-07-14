

- Disk Arbitration
-  DiskArbitration.h 

API Collection

# DiskArbitration.h

Register for mount/unmount notifications, and block mount/unmount events.

## Overview

See the Overview section above for header-level documentation.

## Overview

### Included Headers

- \

- \

- \

- \

## Topics

### Miscellaneous

func DADiskClaim(DADisk, DADiskClaimOptions, DADiskClaimReleaseCallback?, UnsafeMutableRawPointer?, DADiskClaimCallback?, UnsafeMutableRawPointer?)

Claims the specified disk object for exclusive use.

func DADiskEject(DADisk, DADiskEjectOptions, DADiskEjectCallback?, UnsafeMutableRawPointer?)

Ejects the specified disk object.

func DADiskGetOptions(DADisk) -> DADiskOptions

Obtains the options for the specified disk.

func DADiskIsClaimed(DADisk) -> Bool

Reports whether or not the disk is claimed.

func DADiskMount(DADisk, CFURL?, DADiskMountOptions, DADiskMountCallback?, UnsafeMutableRawPointer?)

Mounts the volume at the specified disk object.

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

func DARegisterDiskUnmountApprovalCallback(DASession, CFDictionary?, DADiskUnmountApprovalCallback, UnsafeMutableRawPointer?)

Registers a callback function to be called whenever a volume is to be unmounted.

func DAUnregisterCallback(DASession, UnsafeMutableRawPointer, UnsafeMutableRawPointer?)

Unregisters a registered callback function.

### Callbacks

See the Overview section above for header-level documentation.

typealias DADiskAppearedCallback

Type of the callback function used by DARegisterDiskAppearedCallback().

typealias DADiskClaimCallback

Type of the callback function used by DADiskClaim().

typealias DADiskClaimReleaseCallback

Type of the callback function used by DADiskClaim().

typealias DADiskDescriptionChangedCallback

Type of the callback function used by DARegisterDiskDescriptionChangedCallback().

typealias DADiskDisappearedCallback

Type of the callback function used by DARegisterDiskDisappearedCallback().

typealias DADiskEjectApprovalCallback

Type of the callback function used by DARegisterDiskEjectApprovalCallback().

typealias DADiskEjectCallback

Type of the callback function used by DADiskEject().

typealias DADiskMountApprovalCallback

Type of the callback function used by DARegisterDiskMountApprovalCallback().

typealias DADiskMountCallback

Type of the callback function used by DADiskMount().

typealias DADiskPeekCallback

Type of the callback function used by DARegisterDiskPeekCallback().

typealias DADiskRenameCallback

Type of the callback function used by DADiskRename().

typealias DADiskUnmountApprovalCallback

Type of the callback function used by DARegisterDiskUnmountApprovalCallback().

typealias DADiskUnmountCallback

Type of the callback function used by DADiskUnmount().

### Constants

Global Variables

DADiskClaimOptions

Options for DADiskClaim().

DADiskEjectOptions

Options for DADiskEject().

typealias DADiskMountOptions

Options for DADiskMount().

typealias DADiskRenameOptions

Options for DADiskRename().

typealias DADiskUnmountOptions

Options for DADiskUnmount().

## See Also

### Reference

DADisk.h

DADissenter.h

DASession.h

DiskArbitration Enumerations

DiskArbitration Constants

DiskArbitration Data Types

