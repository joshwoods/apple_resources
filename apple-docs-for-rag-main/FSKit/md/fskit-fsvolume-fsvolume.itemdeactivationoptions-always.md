

- FSKit
- FSVolume
- FSVolume.ItemDeactivationOptions
-  always 

Type Property

# always

An option to always perform deactivation calls.

macOS 15.4+

``` source
static var always: FSVolume.ItemDeactivationOptions { get }
```

## Discussion

Use this option if the file system needs `deactivateItem` calls in circumstances beyond those covered by forRemovedItems and forPreallocatedItems.

## See Also

### Declaring deactivation options

static var forRemovedItems: FSVolume.ItemDeactivationOptions

An option to process deactivation for open-unlinked items at the moment of last close.

static var forPreallocatedItems: FSVolume.ItemDeactivationOptions

An option to process deactivation for for files with preallocated space.

