

- AppKit
- NSImage
-  NSImage.DynamicRange 

Enumeration

# NSImage.DynamicRange

Describes how High Dynamic Range (HDR) image content displays.

macOS 14.0+

``` source
enum DynamicRange
```

## Overview

Use this type to enable or constrain the display of High Dynamic Range (HDR) in an NSImageView. Displaying HDR content in an NSImageView requires that the NSImage has HDR content in the ITU-R 2100 color space and that the output device has Extended Dynamic Range (EDR) capabilities.

## Topics

### Setting the dynamic range

case standard

Restricts the image content dynamic range to the standard range regardless of the actual range of the image content.

case constrainedHigh

Allows for constrained High Dynamic Range (HDR) image content which is useful for mixing HDR and Standard Dynamic Range (SDR) content.

case high

Allows image content to use extended dynamic range if it has dynamic range content.

case unspecified

Indicates that the dynamic range treatment of the image is unknown or otherwise unspecified.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Enumerations

enum FrameResizePosition

The position along the perimeter of a rectangular frame (its edges and corners) from which it’s resized.

enum NSHorizontalDirection

An absolute direction on the horizontal axis.

enum NSSharingCollaborationMode

Represents the types of sharing (collaborating on an item vs. sending a copy of the item) The share picker supports up to two modes, each of which corresponds to one of these types

enum NSTextCursorAccessoryPlacement

enum NSVerticalDirection

A direction on the vertical axis.

enum NSWritingToolsBehavior

Constants that specify the Writing Tools experience for the underlying view.

struct NSWritingToolsResultOptions

Constants to specify what type of content to allow in Writing Tools suggestions or rewrites.

