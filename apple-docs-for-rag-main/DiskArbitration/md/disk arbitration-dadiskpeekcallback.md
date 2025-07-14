

- Disk Arbitration
-  DADiskPeekCallback 

Type Alias

# DADiskPeekCallback

Type of the callback function used by DARegisterDiskPeekCallback().

Mac Catalyst 13.1+macOS 10.4+

``` source
typealias DADiskPeekCallback = (DADisk, UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`disk`  

A disk object.

`context`  

The user-defined context parameter given to the registration function.

## Discussion

The peek callback functions are called in a specific order, from lowest order to highest order. DADiskClaim() could be used here to claim the disk object and DADiskSetOptions() could be used here to set up options on the disk object.

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

typealias DADiskEjectCallback

Type of the callback function used by DADiskEject().

typealias DADiskMountApprovalCallback

Type of the callback function used by DARegisterDiskMountApprovalCallback().

typealias DADiskMountCallback

Type of the callback function used by DADiskMount().

typealias DADiskRenameCallback

Type of the callback function used by DADiskRename().

typealias DADiskUnmountApprovalCallback

Type of the callback function used by DARegisterDiskUnmountApprovalCallback().

typealias DADiskUnmountCallback

Type of the callback function used by DADiskUnmount().

