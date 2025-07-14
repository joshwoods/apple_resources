

- SpriteKit
-  SKCropNode 

Class

# SKCropNode

A node that masks pixels drawn by its children so that only some pixels are seen.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
class SKCropNode
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
class SKCropNode
```

## Mentioned in 

About Node Drawing Order

## Overview

`SKCropNode` is a container node that you use to crop other nodes in the scene. You add other nodes to a crop node and set the crop node’s maskNode property. For example, here are some ways you might specify a mask:

- An untextured sprite that limits content to a rectangular portion of the scene.

- A textured sprite that works as a precise per-pixel mask.

- A collection of child nodes that form a unique shape.

You can animate the shape or contents of the mask to implement interesting effects such as hiding or revealing.

Tip

Use crop nodes sparingly. Because they require an additional offscreen memory buffer to perform the crop and add a rendering operation into the offscreen buffer, they add notably more overhead to the app.

## Topics

### First Steps

Crop other nodes in the scene by adding them as child nodes to a crop node.

Cropping Nodes

Use a texture or a shape to mask pixels out of a crop node’s children.

### Setting the Mask Filter

var maskNode: SKNode?

The node used to determine the crop node’s mask.

## Relationships

### Inherits From

- SKNode

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- Sendable
- UIActivityItemsConfigurationProviding
- UICoordinateSpace
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIUserActivityRestoring

## See Also

### Nodes that Modify Drawing

class SKEffectNode

A node that renders its children into a separate buffer, optionally applying an effect, before drawing the final result.

class SKTransformNode

A node that allows its children to rotate in 3D.

