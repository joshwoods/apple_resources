

- AppKit
- NSWindow
-  disableSnapshotRestoration() 

Instance Method

# disableSnapshotRestoration()

Disables snapshot restoration.

macOS

``` source
@MainActor
func disableSnapshotRestoration()
```

## Discussion

After disabling snapshot restoration, the system doesn’t snapshot the window’s restorable state.

## See Also

### Handling Window Restoration

var isRestorable: Bool

A Boolean value indicating whether the window configuration is preserved between application launches.

var restorationClass: (any NSWindowRestoration.Type)?

The restoration class associated with the window.

func enableSnapshotRestoration()

Enables snapshot restoration.

