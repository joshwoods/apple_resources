

- AppKit
- NSMenuItem
-  keyEquivalentModifierMask 

Instance Property

# keyEquivalentModifierMask

The menu item’s keyboard equivalent modifiers.

macOS

``` source
var keyEquivalentModifierMask: NSEvent.ModifierFlags { get set }
```

## Discussion

`NSShiftKeyMask` is a valid modifier for any key equivalent in `mask`. This allows you to specify key-equivalents such as Command-Shift-1 that are consistent across all keyboards. However, with a few exceptions (such as the German “ß” character), a lowercase character with `NSShiftKeyMask` is interpreted the same as the uppercase character without that mask. For example, Command-Shift-c and Command-C are considered to be identical key equivalents.

See the NSEvent class specification for more information about modifier mask values.

## See Also

### Managing key equivalents

var keyEquivalent: String

The menu item’s unmodified key equivalent.

