

- AppKit
-  NSColorSampler 

Class

# NSColorSampler

An object that displays the system’s color-sampling interface and returns the selected color to your app.

macOS 10.15+

``` source
class NSColorSampler
```

## Overview

Create an NSColorSampler object when you want the user to select a color based on existing onscreen colors. When you call the show(selectionHandler:) method, AppKit shows the system’s color sampler interface and reports the selected color back to the provided block.

## Topics

### Capturing a Color Sample

func show(selectionHandler: (NSColor?) -> Void)

Displays the system color-sampling interface asynchronously and reports the selected color back to your app.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

