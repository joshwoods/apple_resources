

- CarPlay
-  CPContentStyle 

Structure

# CPContentStyle

The types of content style that the vehicle allows.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
struct CPContentStyle
```

## Overview

The vehicle selects the content style according to the ambient light level. Your navigation app can use this value to determine the most appropriate style of map content to draw in its base view. The content style is independent of the user interface style, which controls light and dark mode.

You don’t create instances of `CPContentStyle`. Instead, the session configuration provides the current content style, and it notifies its delegate of any changes. See CPSessionConfiguration for more information.

## Topics

### Creating a Content Style

init(rawValue: UInt)

Creates a content style from a raw value.

### Content Styles

static var dark: CPContentStyle

The indication from the vehicle to draw the content in a dark style.

static var light: CPContentStyle

The indication from the vehicle to draw the content in a light style.

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

### Getting the Content Style

var contentStyle: CPContentStyle

The content style that the vehicle selects.

