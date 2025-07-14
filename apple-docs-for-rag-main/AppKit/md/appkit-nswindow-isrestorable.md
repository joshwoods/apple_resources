

- AppKit
- NSWindow
-  isRestorable 

Instance Property

# isRestorable

A Boolean value indicating whether the window configuration is preserved between application launches.

macOS 10.7+

``` source
@MainActor
var isRestorable: Bool { get set }
```

## Discussion

Set this property to true if you want the window to be preserved or false if you do not want it preserved. By default, the value of this property is true if the window’s styleMask property includes the NSTitledWindowMask flag. For other windows, the value is false. Setting a value explicitly overrides the default values.

Windows should be preserved between launch cycles to maintain interface continuity for the user. During subsequent launch cycles, the system tries to recreate the window and restore its configuration to the preserved state. Configuration data is updated as needed and saved automatically by the system.

If you enable preservation for a given window, you should also specify a restoration class for the window using the restorationClass property.

## See Also

### Handling Window Restoration

var restorationClass: (any NSWindowRestoration.Type)?

The restoration class associated with the window.

func disableSnapshotRestoration()

Disables snapshot restoration.

func enableSnapshotRestoration()

Enables snapshot restoration.

