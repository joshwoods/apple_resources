

- AppKit
- NSFontPanel
-  reloadDefaultFontFamilies() 

Instance Method

# reloadDefaultFontFamilies()

Triggers a reload to the default state, so that the delegate is called.

macOS

``` source
@MainActor
func reloadDefaultFontFamilies()
```

## Discussion

This reloading provides the delegate opportunity to scrutinize the default list of fonts to be displayed in the panel.

## See Also

### Enabling Font Changes

var isEnabled: Bool

A Boolean that shows whether the receiver’s Set button is enabled.

