

- AppKit
- NSWindow
-  NSWindow.CollectionBehavior 

Structure

# NSWindow.CollectionBehavior

Window collection behaviors related to Mission Control, Spaces, and Stage Manager.

macOS 10.5+

``` source
struct CollectionBehavior
```

## Overview

Collection behaviors are properties you set on windows to control their display characteristics in window management technologies. Use them to specify a preference on how windows behave in window management technologies like Mission Control, Spaces, and Stage Manager.

To set a collection behavior on a window, assign one or more behavior options to the window’s collectionBehavior property:

- Swift
- Objective-C

```
window.collectionBehavior = .primary
```

```
window.collectionBehavior = NSWindowCollectionBehaviorPrimary;
```

Not all collection behaviors apply to all windowing management technologies, and some are mutually exclusive to their respective groups. For example, primary, auxiliary, and canJoinAllApplications only apply to full screen and Stage Manager. They’re also mutually exclusive. Specify at most one per window.

## Topics

### Window Collection Behaviors Creation

init(rawValue: UInt)

Creates a window collection behavior using the given raw value.

### Stage Manager and full screen

static var primary: NSWindow.CollectionBehavior

The behavior marking this window as primary for both Stage Manager and full screen.

static var auxiliary: NSWindow.CollectionBehavior

The behavior marking this window as auxiliary for both Stage Manager and full screen.

static var canJoinAllApplications: NSWindow.CollectionBehavior

The behavior marking this window as one that can join all apps for both Stage Manager and full screen.

### Spaces

static var canJoinAllSpaces: NSWindow.CollectionBehavior

The window can appear in all spaces.

static var moveToActiveSpace: NSWindow.CollectionBehavior

When the window becomes active, move it to the active space instead of switching spaces.

### Mission Control

static var stationary: NSWindow.CollectionBehavior

Mission Control doesn’t affect the window, so it stays visible and stationary, like the desktop window.

### Spaces and Mission Control

static var managed: NSWindow.CollectionBehavior

The window participates in Mission Control and Spaces.

static var transient: NSWindow.CollectionBehavior

The window floats in Spaces and hides in Mission Control.

### Full screen

static var fullScreenPrimary: NSWindow.CollectionBehavior

The window can enter full-screen mode.

static var fullScreenAuxiliary: NSWindow.CollectionBehavior

The window displays on the same space as the full screen window.

static var fullScreenNone: NSWindow.CollectionBehavior

The window doesn’t support full-screen mode.

static var fullScreenAllowsTiling: NSWindow.CollectionBehavior

The window can be a secondary full screen tile even if it can’t be a full screen window itself.

static var fullScreenDisallowsTiling: NSWindow.CollectionBehavior

The window doesn’t support being a full-screen tile window, but may support being a full-screen window.

### Window cycling

static var participatesInCycle: NSWindow.CollectionBehavior

The window participates in the window cycle for use with the Cycle Through Windows menu item.

static var ignoresCycle: NSWindow.CollectionBehavior

The window isn’t part of the window cycle for use with the Cycle Through Windows menu item.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

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

enum AnimationBehavior

Constants that control the automatic window animation behavior windows use when ordering to the front or out of view.

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

