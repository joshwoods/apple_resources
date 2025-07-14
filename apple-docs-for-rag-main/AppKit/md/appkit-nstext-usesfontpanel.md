

- AppKit
- NSText
-  usesFontPanel 

Instance Property

# usesFontPanel

A Boolean that controls whether the receiver uses the Font panel and Font menu.

macOS

``` source
@MainActor
var usesFontPanel: Bool { get set }
```

## Discussion

If `flag` is true, the receiver responds to messages from the Font panel and from the Font menu and updates the Font panel with the selection font whenever it changes. If `flag` is false the receiver doesn’t do any of these actions.

