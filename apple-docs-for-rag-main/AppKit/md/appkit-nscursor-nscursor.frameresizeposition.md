

- AppKit
- NSCursor
-  NSCursor.FrameResizePosition 

Enumeration

# NSCursor.FrameResizePosition

The position along the perimeter of a rectangular frame (its edges and corners) from which it’s resized.

Mac Catalyst 18.0+macOS 15.0+

``` source
@frozen
enum FrameResizePosition
```

## Topics

### Enumeration Cases

case bottom

The bottom edge of the frame.

case bottomLeft

The bottom left corner of the frame.

case bottomRight

The bottom right corner of the frame.

case left

The left edge of the frame.

case right

The right edge of the frame.

case top

The top edge of the frame.

case topLeft

The top left corner of the frame.

case topRight

The top right corner of the frame.

### Initializers

init?(rawValue: UInt)

### Type Methods

static func bottomLeading(relativeTo: NSUserInterfaceLayoutDirection) -> NSCursor.FrameResizePosition

The bottom leading corner of the frame, in the given user interface layout direction.

static func bottomTrailing(relativeTo: NSUserInterfaceLayoutDirection) -> NSCursor.FrameResizePosition

The bottom trailing corner of the frame, in the given user interface layout direction.

static func leading(relativeTo: NSUserInterfaceLayoutDirection) -> NSCursor.FrameResizePosition

The leading edge of the frame, in the given user interface layout direction.

static func topLeading(relativeTo: NSUserInterfaceLayoutDirection) -> NSCursor.FrameResizePosition

The top leading corner of the frame, in the given user interface layout direction.

static func topTrailing(relativeTo: NSUserInterfaceLayoutDirection) -> NSCursor.FrameResizePosition

The top trailing corner of the frame, in the given user interface layout direction.

static func trailing(relativeTo: NSUserInterfaceLayoutDirection) -> NSCursor.FrameResizePosition

The trailing edge of the frame, in the given user interface layout direction.

## Relationships

### Conforms To

- BitwiseCopyable
- CaseIterable
- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Enumerations

enum NSHorizontalDirection

An absolute direction on the horizontal axis.

enum NSSharingCollaborationMode

Represents the types of sharing (collaborating on an item vs. sending a copy of the item) The share picker supports up to two modes, each of which corresponds to one of these types

enum DynamicRange

Describes how High Dynamic Range (HDR) image content displays.

enum NSTextCursorAccessoryPlacement

enum NSVerticalDirection

A direction on the vertical axis.

enum NSWritingToolsBehavior

Constants that specify the Writing Tools experience for the underlying view.

struct NSWritingToolsResultOptions

Constants to specify what type of content to allow in Writing Tools suggestions or rewrites.

