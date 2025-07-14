

- SwiftUI
- KeyboardShortcut
- KeyboardShortcut.Localization
-  custom 

Type Property

# custom

Don’t use automatic shortcut remapping.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
static let custom: KeyboardShortcut.Localization
```

## Discussion

When you use this mode, you have to take care of international use-cases separately.

## See Also

### Getting localization strategies

static let automatic: KeyboardShortcut.Localization

Remap shortcuts to their international counterparts, mirrored for right-to-left usage if appropriate.

static let withoutMirroring: KeyboardShortcut.Localization

Don’t mirror shortcuts.

