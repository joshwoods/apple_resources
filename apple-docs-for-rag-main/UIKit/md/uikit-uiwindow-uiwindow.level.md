

- UIKit
- UIWindow
-  UIWindow.Level 

Structure

# UIWindow.Level

The positioning of windows relative to each other.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
struct Level
```

## Overview

The stacking of levels takes precedence over the stacking of windows within each level. That is, even the bottom window in a level obscures the top window of the next level down. Levels are listed in order from lowest to highest.

## Topics

### Window levels

static let normal: UIWindow.Level

The default level.

static let statusBar: UIWindow.Level

The level for a status window.

static let alert: UIWindow.Level

The level for an alert view.

### Initializers

init(CGFloat)

Creates a window level structure.

init(rawValue: CGFloat)

Creates a window level structure with the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Comparable
- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring the window

var rootViewController: UIViewController?

The root view controller for the window.

var windowLevel: UIWindow.Level

The position of the window in the z-axis.

var canResizeToFitContent: Bool

A Boolean value that indicates whether the window’s constraint-based content determines its size.

var screen: UIScreen

The screen to display the window on.

Deprecated

