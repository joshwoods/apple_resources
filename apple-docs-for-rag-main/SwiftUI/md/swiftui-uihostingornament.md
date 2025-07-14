

- SwiftUI
-  UIHostingOrnament 

Class

# UIHostingOrnament

A model that represents an ornament suitable for being hosted in UIKit.

visionOS 1.0+

``` source
class UIHostingOrnament where Content : View
```

## Overview

Use a `UIHostingOrnament` when you want to add ornaments to a UIKit view controller. For example, the following adds a single bottom ornament to the current view controller:

```
self.ornaments = [
    UIHostingOrnament(sceneAnchor: .bottom) {
        OrnamentContent()
    }
]
```

## Topics

### Creating a hosting ornament

var rootView: Content

The root view of the SwiftUI view hierarchy managed by this ornament.

### Setting the alignment

var contentAlignment: Alignment

The alignment in the ornament used to position it.

### Initializers

init(sceneAnchor: UnitPoint, contentAlignment: Alignment, content: () -> Content)

Creates an ornament with the specified alignment and content.

### Instance Properties

var sceneAnchor: UnitPoint

The anchor point for aligning the ornament’s content (based on the `contentAlignment`) with the scene.

## Relationships

### Inherits From

- UIOrnament

## See Also

### Hosting an ornament in UIKit

class UIOrnament

The abstract base class that represents an ornament.

