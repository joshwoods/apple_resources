

- Disk Arbitration
-  DADiskDescriptionChangedCallback 

Type Alias

# DADiskDescriptionChangedCallback

Type of the callback function used by DARegisterDiskDescriptionChangedCallback().

Mac Catalyst 13.1+macOS 10.4+

``` source
typealias DADiskDescriptionChangedCallback = (DADisk, CFArray, UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`disk`  

A disk object.

`keys`  

A list of changed keys.

`context`  

The user-defined context parameter given to the registration function.

## See Also

### Callbacks

typealias DADiskAppearedCallback

Type of the callback function used by DARegisterDiskAppearedCallback().

typealias DADiskClaimCallback

Type of the callback function used by DADiskClaim().

typealias DADiskClaimReleaseCallback

Type of the callback function used by DADiskClaim().

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

