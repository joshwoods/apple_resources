

- AppKit
- NSOpenSavePanelDelegate
-  panel(\_:displayNameFor:) 

Instance Method

# panel(\_:displayNameFor:)

`NSSavePanel`: Optional — Sent when the content type popup is displayed and the save panel needs the display name for a type. If `nil` is returned, the save panel will display type’s `localizedDescription`. `NSOpenPanel`: Not sent.

macOS 15.0+

``` source
@MainActor
optional func panel(
    _ sender: Any,
    displayNameFor type: UTType
) -> String?
```

