

- UIKit
- UIButton
- UIButton.Configuration
-  UIButton.Configuration.Size 

Enumeration

# UIButton.Configuration.Size

A predefined size for button elements.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
enum Size
```

## Overview

You can use this enumeration to choose a predefined size for elements in a button. The value you choose for button size can be effectively overridden by explicitly assigning values for configuration elements like padding, corner style, or title and subtitle font sizes.

## Topics

### Button sizes

case large

Displays button elements at a large size.

case medium

Displays button elements at a standard size.

case small

Displays button elements at a small size.

case mini

Displays button elements at the smallest size.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Configuring layout

var buttonSize: UIButton.Configuration.Size

A size that requests a preferred size for the button.

var contentInsets: NSDirectionalEdgeInsets

The distance from the button’s content area to its bounds.

func setDefaultContentInsets()

Restores the default content insets.

