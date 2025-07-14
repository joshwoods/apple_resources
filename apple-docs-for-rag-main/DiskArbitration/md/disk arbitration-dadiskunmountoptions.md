

- Disk Arbitration
-  DADiskUnmountOptions 

Type Alias

# DADiskUnmountOptions

Options for DADiskUnmount().

Mac Catalyst 13.0+macOS 10.4+

``` source
typealias DADiskUnmountOptions = UInt32
```

## Topics

### Constants

var kDADiskUnmountOptionForce: Int

Unmount the volume even if files are still active.

var kDADiskUnmountOptionWhole: Int

Unmount the volumes tied to the whole disk object.

## See Also

### Data Types

typealias DADiskClaimOptions

Options for DADiskClaim().

typealias DADiskEjectOptions

Options for DADiskEject().

typealias DADiskMountOptions

Options for DADiskMount().

typealias DADiskOptions

Options for DADiskGetOptions() and DADiskSetOptions().

typealias DADiskRenameOptions

Options for DADiskRename().

typealias DAReturn

A return code.

