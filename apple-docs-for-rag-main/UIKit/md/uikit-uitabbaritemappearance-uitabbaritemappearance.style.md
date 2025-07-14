

- UIKit
- UITabBarItemAppearance
-  UITabBarItemAppearance.Style 

Enumeration

# UITabBarItemAppearance.Style

Constants indicating the layout of a tab bar item’s content.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum Style
```

## Overview

A tab bar adjusts the layout of each item’s icon and title string based on the current trait environment and other factors.

## Topics

### Item layout

case stacked

A vertically stacked icon and title.

case inline

A side-by-side layout of the icon and title, suitable for use in regular-width environments.

case compactInline

A side-by-side layout of the icon and title, suitable for use in compact-width environments.

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

### Resetting the appearance properties

func configureWithDefault(for: UITabBarItemAppearance.Style)

Configures the tab bar item appearance object with appropriate values for the specified style.

