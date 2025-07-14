

- AppKit
- NSPanel
-  worksWhenModal 

Instance Property

# worksWhenModal

A Boolean value that indicates whether the panel receives keyboard and mouse events even when some other window is being run modally.

macOS

``` source
@MainActor
var worksWhenModal: Bool { get set }
```

## Discussion

The value of this property is true when the panel receives keyboard and mouse events even when some other window is being run modally; when the value is false, the panel is prevented from receiving events while a modal loop or session is running. By default, the value of this property is false, indicating a panel’s ineligibility for events during a modal loop or session. See How Modal Windows Work for more information on modal windows and panels.

## See Also

### Related Documentation

func runModalSession(NSApplication.ModalSession) -> NSApplication.ModalResponse

Runs a given modal session, as defined in a previous invocation of beginModalSession(for:).

func runModal(for: NSWindow) -> NSApplication.ModalResponse

Starts a modal event loop for the specified window.

### Configuring Panels

var isFloatingPanel: Bool

A Boolean value that indicates whether the receiver is a floating panel.

var becomesKeyOnlyIfNeeded: Bool

A Boolean value that indicates whether the receiver becomes the key window only when needed.

