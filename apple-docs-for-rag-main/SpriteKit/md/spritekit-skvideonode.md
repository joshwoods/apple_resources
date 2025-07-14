

- SpriteKit
-  SKVideoNode 

Class

# SKVideoNode

A graphical element that plays video content.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
class SKVideoNode
```

**watchOS**

``` source
class SKVideoNode
```

## Mentioned in 

Adding a Video to a Scene

Animate the Warping of a Sprite

## Overview

This class renders a video at a given size and location in your scene with no exposed player controls.

## Topics

### Getting Started with Video

Adding a Video to a Scene

Play video in your scene by adding a video node.

### Creating a Video Node

init(avPlayer: AVPlayer)

Initializes a video node using an existing AVPlayer object.

init(fileNamed: String)

Initializes a video node using a video file stored in the app bundle.

init(url: URL)

Initializes a video node using a URL.

init?(coder: NSCoder)

Tells you when to initialize a video node that was created from an archive.

init(videoFileNamed: String)

Initializes a video node using a video file stored in the app bundle.

Deprecated

init(videoURL: URL)

Initializes a video node using a URL that points to a video file.

Deprecated

### Setting the Video Node’s Visual Properties

var anchorPoint: CGPoint

The point in the sprite that corresponds to the node’s position.

var size: CGSize

The dimensions of the video node, in points.

### Controlling Video Playback

func play()

Starts video playback.

func pause()

Pauses video playback.

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

### Nodes that Draw

Maximizing Node Drawing Performance

Structure your nodes for maximum performance.

class SKSpriteNode

An image or solid color.

class SKShapeNode

A mathematical shape that can be stroked or filled.

class SKEmitterNode

A source of various particle effects.

class SKLabelNode

A graphical element that draws text.

class SKTileMapNode

A two-dimensional array of images.

class SK3DNode

3D SceneKit content drawn as a flattened sprite.

