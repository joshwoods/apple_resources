

- AppKit
- NSToolbar
-  runCustomizationPalette(\_:) 

Instance Method

# runCustomizationPalette(\_:)

Displays the toolbar’s customization palette and handles any user-initiated customizations.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
@MainActor
func runCustomizationPalette(_ sender: Any?)
```

## Parameters 

`sender`  

The control sending the message.

## Discussion

While the customization palette is visible, the toolbar calls methods of its delegate to manage configuration changes.

## See Also

### Displaying the customization palette

var customizationPaletteIsRunning: Bool

A Boolean value that indicates whether the toolbar’s customization palette is in use.

