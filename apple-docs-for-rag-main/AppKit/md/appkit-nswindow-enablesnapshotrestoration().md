

- AppKit
- NSWindow
-  enableSnapshotRestoration() 

Instance Method

# enableSnapshotRestoration()

Enables snapshot restoration.

macOS

``` source
@MainActor
func enableSnapshotRestoration()
```

## Discussion

While snapshot restoration is enabled, the system snapshots the window’s restorable state.

## See Also

### Handling Window Restoration

var isRestorable: Bool

A Boolean value indicating whether the window configuration is preserved between application launches.

var restorationClass: (any NSWindowRestoration.Type)?

The restoration class associated with the window.

func disableSnapshotRestoration()

Disables snapshot restoration.

