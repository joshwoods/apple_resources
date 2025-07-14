

- FSKit
- FSVolume
- FSVolume.ItemDeactivationOptions
-  forRemovedItems 

Type Property

# forRemovedItems

An option to process deactivation for open-unlinked items at the moment of last close.

macOS 15.4+

``` source
static var forRemovedItems: FSVolume.ItemDeactivationOptions { get }
```

## See Also

### Declaring deactivation options

static var forPreallocatedItems: FSVolume.ItemDeactivationOptions

An option to process deactivation for for files with preallocated space.

static var always: FSVolume.ItemDeactivationOptions

An option to always perform deactivation calls.

