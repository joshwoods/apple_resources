

- AppKit
- NSColorPicker
-  setMode(\_:) 

Instance Method

# setMode(\_:)

Overriden to set the color picker’s mode.

macOS

``` source
@MainActor
func setMode(_ mode: NSColorPanel.Mode)
```

## Parameters 

`mode`  

A constant specifying the color picking mode. These constants are defined in `AppKit/NSColorPanel.h`.

## Discussion

In grayscale-alpha, red-green-blue, cyan-magenta-yellow-black, and hue-saturation-brightness modes, the user adjusts colors by manipulating sliders. In the custom palette mode, the user can load an `NSImage` file (TIFF or EPS) into the `NSColorPanel`, then select colors from the image. In custom color list mode, the user can create and load lists of named colors. The two custom modes provide `NSPopUpList`s for loading and saving files. Finally, color wheel mode provides a simplified control for selecting colors.

