

- AppKit
- NSOpenSavePanelDelegate
-  panel(\_:didSelect:) 

Instance Method

# panel(\_:didSelect:)

`NSSavePanel`: Optional — Sent when the user changes the current type. `NSOpenPanel`: Not sent.

macOS 15.0+

``` source
@MainActor
optional func panel(
    _ sender: Any,
    didSelect type: UTType?
)
```

