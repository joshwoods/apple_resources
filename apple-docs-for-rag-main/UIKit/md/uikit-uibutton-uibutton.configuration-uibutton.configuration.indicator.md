

- UIKit
- UIButton
- UIButton.Configuration
-  UIButton.Configuration.Indicator 

Enumeration

# UIButton.Configuration.Indicator

Constants that determine the style of the indicator that appears on a button.

iOS 16.0+iPadOS 16.0+Mac CatalysttvOS 16.0+visionOS

``` source
enum Indicator
```

## Overview

Use these constants to set the value of the indicator property.

## Topics

### Indicator styles

case automatic

A constant that automatically determines an indicator style according to the button’s properties.

case none

A constant that doesn’t show an indicator.

case popup

A constant that shows a popup-style indicator.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Configuring the indicator

var indicator: UIButton.Configuration.Indicator

The style of the indicator that appears on the button.

var indicatorColorTransformer: UIConfigurationColorTransformer?

The color transformer for resolving the indicator color.

