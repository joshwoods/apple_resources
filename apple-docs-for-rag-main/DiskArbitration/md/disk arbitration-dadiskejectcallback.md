

- Disk Arbitration
-  DADiskEjectCallback 

Type Alias

# DADiskEjectCallback

Type of the callback function used by DADiskEject().

Mac Catalyst 13.1+macOS 10.4+

``` source
typealias DADiskEjectCallback = (DADisk, DADissenter?, UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`disk`  

The disk object.

`dissenter`  

A dissenter object on failure or NULL on success.

`context`  

The user-defined context parameter given to the eject function.

## See Also

### Callbacks

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

