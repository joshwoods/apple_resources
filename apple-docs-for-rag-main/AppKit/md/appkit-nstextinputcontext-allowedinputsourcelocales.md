

- AppKit
- NSTextInputContext
-  allowedInputSourceLocales 

Instance Property

# allowedInputSourceLocales

The set of keyboard input source locales allowed when this input context is active.

macOS 10.6+

``` source
var allowedInputSourceLocales: [String]? { get set }
```

## Discussion

`NSAllRomanInputSourcesLocaleIdentifier` can be specified as a valid locale.

## See Also

### Configuring the Input Context

var acceptsGlyphInfo: Bool

A Boolean value that indicates whether the client handles `NSGlyphInfoAttributeName` or not.

