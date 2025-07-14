

- AppKit
- NSWindow
-  NSWindow.OrderingMode 

Enumeration

# NSWindow.OrderingMode

Constants that let you specify how a window is ordered relative to another window.

macOS

``` source
enum OrderingMode
```

## Overview

For more information, see order(_:relativeTo:).

## Topics

### Constants

case above

Moves the window above the indicated window.

case below

Moves the window below the indicated window.

case out

Moves the window off the screen.

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

### Constants

enum SelectionDirection

Constants that specify the direction a window is currently using to change the key view.

enum ButtonType

Constants that provide a way to access standard title bar buttons.

NSRunLoop—Ordering Modes for NSWindow

Constants that specify the priority for runloop messages.

enum Depth

A type that represents the depth, or amount of memory, for a single pixel in a window or screen.

enum BackingStoreType

Constants that specify how the window device buffers the drawing done in a window.

enum SharingType

Constants that represent the access levels other processes can have to a window’s content.

struct NumberListOptions

Options to use when retrieving window numbers from the system.

enum AnimationBehavior

Constants that control the automatic window animation behavior windows use when ordering to the front or out of view.

struct CollectionBehavior

Window collection behaviors related to Mission Control, Spaces, and Stage Manager.

struct OcclusionState

Specifies whether the window is occluded.

enum TitleVisibility

Specifies the appearance of the window’s title bar area.

enum UserTabbingPreference

A value that indicates the user’s preference for window tabbing.

enum TabbingMode

The preferred tabbing behavior of a window.

Application Kit Version for Deferred Window Display Support

The version of the AppKit.framework containing a specific bug fix or capability.

Application Kit Version for Custom Sheet Position

The version of the AppKit.framework containing a specific bug fix or capability.

