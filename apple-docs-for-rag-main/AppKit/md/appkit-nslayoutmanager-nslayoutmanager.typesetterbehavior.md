

- AppKit
- NSLayoutManager
-  NSLayoutManager.TypesetterBehavior 

Enumeration

# NSLayoutManager.TypesetterBehavior

Constants that determine the layout manager’s behavior during layout.

macOS

``` source
enum TypesetterBehavior
```

## Overview

These constants define the behavior of `NSLayoutManager` and `NSTypesetter` when laying out lines. They are used by typesetterBehavior to control the compatibility level of the typesetter.

## Topics

### Behaviors

case latestBehavior

The current typesetter behavior in the current operating system.

case originalBehavior

The original typesetter behavior, as shipped with macOS 10.1 and earlier.

case behavior_10_2_WithCompatibility

The macOS 10.2 typesetting behavior that is still compatible with the original typesetter behavior.

case behavior_10_2

The typesetter behavior introduced in macOS 10.2.

case behavior_10_3

The typesetter behavior introduced in macOS 10.3.

case behavior_10_4

The typesetter behavior introduced in macOS 10.4.

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

### Managing the typesetter

var typesetter: NSTypesetter

The current typesetter.

var typesetterBehavior: NSLayoutManager.TypesetterBehavior

The default typesetter behavior.

func defaultLineHeight(for: NSFont) -> CGFloat

Returns the default line height for a line of text that uses a specified font.

func defaultBaselineOffset(for: NSFont) -> CGFloat

Returns the default baseline offset that the layout manager’s typesetter uses for the specified font.

