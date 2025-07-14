

- AppKit
- NSWindow
-  NSWindow.BackingStoreType 

Enumeration

# NSWindow.BackingStoreType

Constants that specify how the window device buffers the drawing done in a window.

macOS

``` source
enum BackingStoreType
```

## Topics

### Constants

case retained

The window uses a buffer, but draws directly to the screen where possible and to the buffer for obscured portions.

Deprecated

case nonretained

The window draws directly to the screen without using any buffer.

Deprecated

case buffered

The window renders all drawing into a display buffer and then flushes it to the screen.

### Initializers

init?(rawValue: UInt)

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

enum OrderingMode

Constants that let you specify how a window is ordered relative to another window.

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

