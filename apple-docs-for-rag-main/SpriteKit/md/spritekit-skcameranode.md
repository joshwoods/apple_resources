

- SpriteKit
-  SKCameraNode 

Class

# SKCameraNode

A node that determines which parts of the scene are visible within a view.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

**watchOS**

``` source
class SKCameraNode
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
class SKCameraNode
```

## Mentioned in 

Positioning a Scene’s Origin Within its View

Using Base Nodes to Lay Out SpriteKit Content

## Overview

If you don’t use a camera in your scene, you control the visible portion of a scene using its anchorPoint property.

## Topics

### First Steps

Getting Started with a Camera

Learn the semantics of using a camera in your scene.

### Node Visibility

Check whether a particular node is onscreen.

func containedNodeSet() -> Set&lt;SKNode>

Finds nodes that are visible in the camera’s viewport.

func contains(SKNode) -> Bool

Checks to see if a node is visible in the camera’s viewport.

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

### Base Nodes

Using Base Nodes to Lay Out SpriteKit Content

Use nonvisual nodes to define the layout of a scene.

class SKNode

The base class of all SpriteKit nodes.

class SKReferenceNode

A node that’s defined in an archived `.sks` file.

