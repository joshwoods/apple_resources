

- AppKit
- NSFontPanel
-  sharedFontPanelExists 

Type Property

# sharedFontPanelExists

Returns true if the shared Font panel has been created, false if it hasn’t.

macOS

``` source
@MainActor
class var sharedFontPanelExists: Bool { get }
```

## See Also

### Getting the Font Panel

class var shared: NSFontPanel

Returns the single `NSFontPanel` instance for the application, creating it if necessary.

