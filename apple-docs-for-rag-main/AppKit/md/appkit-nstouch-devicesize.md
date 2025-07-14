

- AppKit
- NSTouch
-  deviceSize 

Instance Property

# deviceSize

The range of the touch device in points, such as 72 ppi.

macOS 10.6+

``` source
var deviceSize: NSSize { get }
```

## Discussion

The lower-left corner of the surface is considered (0,0).

## See Also

### Using Touch Device Properties

var device: Any?

The digitizer that generates the touch. Useful to distinguish touches emanating from multiple-device scenarios.

