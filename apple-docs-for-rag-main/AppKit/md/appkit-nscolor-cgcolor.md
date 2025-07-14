

- AppKit
- NSColor
-  cgColor 

Instance Property

# cgColor

The Core Graphics color object corresponding to the color.

macOS 10.8+

``` source
var cgColor: CGColor { get }
```

## Discussion

This property always contains a valid color, even though the value may be an approximation in some cases. There is no guaranteed round-trip color fidelity.

