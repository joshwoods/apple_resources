

- ImageCaptureCore
- ICScannerDevice
-  defaultUsername 

Instance Property

# defaultUsername

A default username on protected scanners.

macOS 10.4+

``` source
var defaultUsername: String { get set }
```

## Discussion

If the scanner is protected, you can set this property to a specific username as a convenience, instead of prompting the user for a username. The value persists until reset to `nil`.

