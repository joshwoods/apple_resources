

- Disk Arbitration
-  DADiskUnmountApprovalCallback 

Type Alias

# DADiskUnmountApprovalCallback

Type of the callback function used by DARegisterDiskUnmountApprovalCallback().

Mac Catalyst 13.1+macOS 10.4+

``` source
typealias DADiskUnmountApprovalCallback = (DADisk, UnsafeMutableRawPointer?) -> Unmanaged?
```

## Parameters 

`disk`  

A disk object.

`context`  

The user-defined context parameter given to the registration function.

## Return Value

A dissenter reference. Pass NULL to approve.

## Discussion

The caller of this callback receives a reference to the returned object. The caller also implicitly retains the object and is responsible for releasing it with CFRelease().

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

typealias DADiskPeekCallback

Type of the callback function used by DARegisterDiskPeekCallback().

typealias DADiskRenameCallback

Type of the callback function used by DADiskRename().

typealias DADiskUnmountCallback

Type of the callback function used by DADiskUnmount().

