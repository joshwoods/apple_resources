

- AppKit
- NSWindow
-  NSWindow.Depth 

Enumeration

# NSWindow.Depth

A type that represents the depth, or amount of memory, for a single pixel in a window or screen.

macOS 10.6+

``` source
enum Depth
```

## Overview

A depth of `0` indicates default depth. Don’t make window depths persistent because they aren’t the same across systems.

Use the functions colorSpaceName, bitsPerPixel, and isPlanar to extract info from an `NSWindowDepth` value.

Use NSBestDepth to compute window depths. NSBestDepth tries to accommodate all the parameters (match or better). If there are multiple matches, this function uses color space first, then bits per sample (`bps`), then `planar`, then bits per pixel (`bpp)` to determine the closest match. Use `0` for `bpp` to indicate the default, the same as the number of bits per plane: either `bps` or `bps` \* numberOfColorComponents. You may use other values as hints to provide backing stores of different configurations — for instance, 8-bit color.

You can also use one of the explicit bit depths defined in `Explicit Window Depth Limits` for the `NSWindow` property depthLimit.

## Topics

### Constants

case onehundredtwentyeightBitRGB

One hundred and twenty eight bit RGB depth limit.

case sixtyfourBitRGB

Sixty four bit RGB depth limit.

case twentyfourBitRGB

Twenty four bit RGB depth limit.

### Accessing Depth Details

static var availableDepths: [NSWindow.Depth]

An array that contains all available windows depths.

static func bestDepth(colorSpaceName: NSColorSpaceName, bitsPerSample: Int, bitsPerPixel: Int, isPlanar: Bool) -> (NSWindow.Depth, isExactMatch: Bool)

Determines the best window depth that most closely matches the given properties.

var bitsPerPixel: Int

Returns the bits per pixel for the specified window depth.

var bitsPerSample: Int

Returns the bits per sample for the specified window depth.

var colorSpaceName: NSColorSpaceName?

Returns the name of the color space corresponding to the passed window depth.

var isPlanar: Bool

Returns whether the specified window depth is planar.

### Initializers

init?(rawValue: Int32)

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

