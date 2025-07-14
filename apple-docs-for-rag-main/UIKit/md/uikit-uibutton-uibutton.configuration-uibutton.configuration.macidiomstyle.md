

- UIKit
- UIButton
- UIButton.Configuration
-  UIButton.Configuration.MacIdiomStyle 

Enumeration

# UIButton.Configuration.MacIdiomStyle

The button style your app uses when running in macOS.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
enum MacIdiomStyle
```

## Overview

If you build your app with Mac Catalyst, you can use these styles to configure how your app displays a button when running on a Mac. To opt in to these styles, choose Optimize Interface for Mac in you project’s general settings.

If you’re configuring your button in Interface Builder, you can choose a style from the Mac Style pop-up menu in the Attributes inspector.

## Topics

### Button styles

case automatic

The button has a style that matches other content in the button configuration.

case bordered

The button has a bordered style.

case borderless

The button has a borderless style.

case borderlessTinted

The button has a tinted, borderless style.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Configuring the appearance on macOS

var macIdiomStyle: UIButton.Configuration.MacIdiomStyle

The style to use when this button appears in macOS.

