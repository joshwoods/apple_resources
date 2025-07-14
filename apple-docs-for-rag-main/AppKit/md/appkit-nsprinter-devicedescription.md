

- AppKit
- NSPrinter
-  deviceDescription 

Instance Property

# deviceDescription

A dictionary of keys and values that describe the device.

macOS

``` source
var deviceDescription: [NSDeviceDescriptionKey : Any] { get }
```

## Return Value

A dictionary of the device properties. See `NSGraphics.h` for possible keys. The only key guaranteed to exist is `NSDeviceIsPrinter`.

