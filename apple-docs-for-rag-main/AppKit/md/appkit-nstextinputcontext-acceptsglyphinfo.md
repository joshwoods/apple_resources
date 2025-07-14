

- AppKit
- NSTextInputContext
-  acceptsGlyphInfo 

Instance Property

# acceptsGlyphInfo

A Boolean value that indicates whether the client handles `NSGlyphInfoAttributeName` or not.

macOS 10.6+

``` source
var acceptsGlyphInfo: Bool { get set }
```

## Discussion

The default value is determined by examining the return value from sending a `validAttributesForMarkedText` message to the client at initialization.

## See Also

### Configuring the Input Context

var allowedInputSourceLocales: [String]?

The set of keyboard input source locales allowed when this input context is active.

