

- AppKit
-  NSWritingToolsBehavior 

Enumeration

# NSWritingToolsBehavior

Constants that specify the Writing Tools experience for the underlying view.

macOS 15.0+

``` source
enum NSWritingToolsBehavior
```

## Overview

Writing Tools provide proofreading and rewriting support for the content of text views. On devices that support Writing Tools features, people engage the system UI to choose how to rewrite all or part of the available text. These constants indicate whether people experience Writing Tools inline with their text, in an overlay panel, or not at all.

## Topics

### Getting the Writing Tools behaviors

case none

An option to prevent Writing Tools from modifying the text in the view.

case `default`

An option to let the system determine the best way to enable Writing Tools for the view.

case complete

An option to provide the complete Writing Tools experience for the text view.

case limited

An option to provide a limited, overlay-panel experience for the text view.

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

enum DynamicRange

Describes how High Dynamic Range (HDR) image content displays.

enum NSTextCursorAccessoryPlacement

enum NSVerticalDirection

A direction on the vertical axis.

struct NSWritingToolsResultOptions

Constants to specify what type of content to allow in Writing Tools suggestions or rewrites.

