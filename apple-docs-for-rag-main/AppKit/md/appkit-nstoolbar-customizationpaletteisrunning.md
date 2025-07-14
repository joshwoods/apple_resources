

- AppKit
- NSToolbar
-  customizationPaletteIsRunning 

Instance Property

# customizationPaletteIsRunning

A Boolean value that indicates whether the toolbar’s customization palette is in use.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
@MainActor
var customizationPaletteIsRunning: Bool { get }
```

## Discussion

The value of this property is true when the toolbar’s customization palette is running; otherwise, it’s false.

## See Also

### Displaying the customization palette

func runCustomizationPalette(Any?)

Displays the toolbar’s customization palette and handles any user-initiated customizations.

