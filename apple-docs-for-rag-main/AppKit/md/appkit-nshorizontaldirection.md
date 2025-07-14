

- AppKit
-  NSHorizontalDirection 

Enumeration

# NSHorizontalDirection

An absolute direction on the horizontal axis.

Mac Catalyst 18.0+macOS 15.0+

``` source
@frozen
enum NSHorizontalDirection
```

## Topics

### Structures

struct Set

An efficient set of horizontal directions.

### Enumeration Cases

case left

The left direction.

case right

The right direction.

### Type Methods

static func leading(relativeTo: NSUserInterfaceLayoutDirection) -> NSHorizontalDirection

Returns the leading direction in the given user interface layout direction.

static func trailing(relativeTo: NSUserInterfaceLayoutDirection) -> NSHorizontalDirection

Returns the trailing direction in the given user interface layout direction.

## Relationships

### Conforms To

- BitwiseCopyable
- CaseIterable
- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Enumerations

enum FrameResizePosition

The position along the perimeter of a rectangular frame (its edges and corners) from which it’s resized.

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

