

- Accessibility
-  AXBrailleMapRenderer 

Protocol

# AXBrailleMapRenderer

The interface for providing data for a braille map.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
protocol AXBrailleMapRenderer : NSObjectProtocol
```

## Overview

You update the braille display in one of these ways:

- Implement accessibilityBrailleMapRenderRegion to specify an area of the UI to render to the braille display. With this approach, VoiceOver handles the process of converting the data to a braille map by rendering the image of the screen in that region and updating the braille display automatically.

- Implement accessibilityBrailleMapRenderer to update the braille map manually. With this approach, you get more detailed control over what to display, but you must modify the braille map yourself.

## Topics

### Rendering a specific region

var accessibilityBrailleMapRenderRegion: CGRect

A region of the UI that the system converts into a braille map and displays on the braille display.

### Updating the braille map manually

var accessibilityBrailleMapRenderer: (AXBrailleMap) -> Void

A handler that the system calls to let you update the Braille map.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Braille maps

class AXBrailleMap

A representation of a two-dimensional braille display.

