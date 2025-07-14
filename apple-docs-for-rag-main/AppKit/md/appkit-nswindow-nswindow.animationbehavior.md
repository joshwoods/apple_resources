

- AppKit
- NSWindow
-  NSWindow.AnimationBehavior 

Enumeration

# NSWindow.AnimationBehavior

Constants that control the automatic window animation behavior windows use when ordering to the front or out of view.

macOS 10.7+

``` source
enum AnimationBehavior
```

## Topics

### Constants

case `default`

The automatic animation that’s appropriate to the window type. This is the default.

case none

No automatic animation used. This may be useful when you perform your own window animation.

case documentWindow

The animation behavior that’s appropriate to the document window style.

case utilityWindow

The animation behavior that’s appropriate to the utility window style.

case alertPanel

The animation behavior that’s appropriate to the alert window style.

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

enum OrderingMode

Constants that let you specify how a window is ordered relative to another window.

enum SharingType

Constants that represent the access levels other processes can have to a window’s content.

struct NumberListOptions

Options to use when retrieving window numbers from the system.

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

