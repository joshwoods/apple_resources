

- FSKit
- FSVolume
- FSVolume.ItemDeactivationOptions
-  forPreallocatedItems 

Type Property

# forPreallocatedItems

An option to process deactivation for for files with preallocated space.

macOS 15.4+

``` source
static var forPreallocatedItems: FSVolume.ItemDeactivationOptions { get }
```

## Discussion

This option facilitates a sort of trim-on-close behavior. It is only meaningful for volumes that conform to FSVolume.PreallocateOperations.

## See Also

### Declaring deactivation options

static var forRemovedItems: FSVolume.ItemDeactivationOptions

An option to process deactivation for open-unlinked items at the moment of last close.

static var always: FSVolume.ItemDeactivationOptions

An option to always perform deactivation calls.

