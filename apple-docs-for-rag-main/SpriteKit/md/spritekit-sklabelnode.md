

- SpriteKit
-  SKLabelNode 

Class

# SKLabelNode

A graphical element that draws text.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
class SKLabelNode
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
class SKLabelNode
```

## Mentioned in 

Warping SpriteKit Content By Using an Effect Node

Getting Started with Nodes

Adding Text to a Scene

## Overview

`SKLabelNode` allows you to render text in your scene. You can define a custom style using properties such as fontName and fontColor, or configure the look of your text with an NSAttributedString.

## Topics

### Getting Started with Labels

Adding Text to a Scene

Draw text in your scene, such as a health indicator or a “Game Over” banner, by using a label node.

### Creating a Label

init(fontNamed: String?)

Initializes a new label object with a specified font.

convenience init(text: String?)

Initializes a new label object with a text string.

convenience init(attributedText: NSAttributedString?)

Initializes a new label object with an attributed text string.

### Setting a Label’s Text

var text: String?

The string that the label node displays.

var attributedText: NSAttributedString?

The attributed string displayed by the label.

### Specifying a Label’s Font

var fontColor: UIColor?

The color of the label.

var fontName: String?

The font used for the text in the label.

var fontSize: CGFloat

The size of the font used in the label.

### Controlling a Label’s Alignment

var verticalAlignmentMode: SKLabelVerticalAlignmentMode

The vertical position of the text within the node.

enum SKLabelVerticalAlignmentMode

Options for aligning text vertically.

var horizontalAlignmentMode: SKLabelHorizontalAlignmentMode

The horizontal position of the text within the node.

enum SKLabelHorizontalAlignmentMode

Options for aligning text horizontally.

### Defining a Label’s Line-Breaking Behavior

Configure these properties to control line-breaking behavior.

var preferredMaxLayoutWidth: CGFloat

The width, in screen points, after which line-break mode should be applied.

var lineBreakMode: NSLineBreakMode

Determines the line-break mode for multiple lines.

var numberOfLines: Int

Determines the number of lines to draw.

### Colorizing a Label

var color: UIColor?

An alternative to the font color that can be used for animations.

var colorBlendFactor: CGFloat

A floating-point value that describes how the color is blended with the font color.

### Configuring Alpha Blending

Change how a label uses an alpha value, such as additive blending, that results in the label being brighter than it was before.

var blendMode: SKBlendMode

The blend mode used to draw the label into the parent’s framebuffer.

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

class SKVideoNode

A graphical element that plays video content.

class SKTileMapNode

A two-dimensional array of images.

class SK3DNode

3D SceneKit content drawn as a flattened sprite.

