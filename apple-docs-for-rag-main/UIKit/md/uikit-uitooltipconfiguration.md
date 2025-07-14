

- UIKit
-  UIToolTipConfiguration 

Class

# UIToolTipConfiguration

An object that a tooltip interaction delegate uses to describe the tooltip settings.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
class UIToolTipConfiguration
```

## Overview

Use a tooltip configuration to specify:

- The text that appears in the tooltip.

- The region that the pointer must hover over to trigger the appearance of the tooltip.

A UIToolTipInteraction object asks for a configuration from its delegate by calling the delegate method toolTipInteraction(_:configurationAt:).

## Topics

### Creating a tooltip configuration

convenience init(toolTip: String)

Creates a tooltip configuration and sets the tooltip text.

convenience init(toolTip: String, in: CGRect)

Creates a tooltip configuration, and sets the tooltip text and hover region within the view or control.

### Accessing the configuration settings

var toolTip: String

The text to display in the tooltip.

var sourceRect: CGRect?

The region of the view or control where the pointer must hover to trigger the appearance of the tooltip.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Providing a tooltip configuration

func toolTipInteraction(UIToolTipInteraction, configurationAt: CGPoint) -> UIToolTipConfiguration?

Asks the delegate for a tooltip configuration that describes the tooltip settings.

