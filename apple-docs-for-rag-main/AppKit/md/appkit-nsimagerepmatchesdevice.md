

- AppKit
-  NSImageRepMatchesDevice 

Global Variable

# NSImageRepMatchesDevice

A constant indicating that the value of certain attributes, such as the number of colors or bits per sample, will change to match the display device.

macOS

``` source
var NSImageRepMatchesDevice: Int { get }
```

## Discussion

This value can be passed in (or received back) as the value of bitsPerSample, pixelsWide, and pixelsHigh.

