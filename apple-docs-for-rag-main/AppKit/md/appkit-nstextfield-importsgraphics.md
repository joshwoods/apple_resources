

- AppKit
- NSTextField
-  importsGraphics 

Instance Property

# importsGraphics

A Boolean value that controls whether the user can drag image files into the text field.

macOS

``` source
@MainActor
var importsGraphics: Bool { get set }
```

## Discussion

If true, the text field accepts dragged images; if false, it doesn’t. You can add images programmatically regardless of this setting.

## See Also

### Controlling Rich Text Behavior

var allowsEditingTextAttributes: Bool

A Boolean value that controls whether the user can change font attributes of the text field’s string.

