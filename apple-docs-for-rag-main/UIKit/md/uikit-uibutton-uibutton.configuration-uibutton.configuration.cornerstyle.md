

- UIKit
- UIButton
- UIButton.Configuration
-  UIButton.Configuration.CornerStyle 

Enumeration

# UIButton.Configuration.CornerStyle

Settings that determine the appearance of the background corner radius.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
enum CornerStyle
```

## Overview

Use this property to control how the button uses the cornerRadius property of the button’s background.

## Topics

### Corner styles

case dynamic

A style that adjusts the background corner radius for dynamic type.

case fixed

A style that uses the background corner radius without modification.

case capsule

A style that ignores the background corner radius and uses a corner radius that generates a capsule.

case large

A style that ignores the background corner radius and uses a large system-defined corner radius.

case medium

A style that ignores the background corner radius and uses a medium system-defined corner radius.

case small

A style that ignores the background corner radius and uses a small system-defined corner radius.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Configuring the button background

var background: UIBackgroundConfiguration

The configuration to customize the button background.

var cornerStyle: UIButton.Configuration.CornerStyle

The button style that controls the display behavior of the background corner radius.

