

- AppKit
- NSFontPanel
-  isEnabled 

Instance Property

# isEnabled

A Boolean that shows whether the receiver’s Set button is enabled.

macOS

``` source
@MainActor
var isEnabled: Bool { get set }
```

## Discussion

The receiver continues to reflect the font of the selection for cooperating text objects regardless of this setting.

## See Also

### Enabling Font Changes

func reloadDefaultFontFamilies()

Triggers a reload to the default state, so that the delegate is called.

