

- CarPlay
-  CPTextButton 

Class

# CPTextButton

A button that displays a stylized title.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class CPTextButton
```

## Overview

You use a text button to attach custom actions to an instance of CPPointOfInterest or CPInformationTemplate. When creating a button, you provide a closure that CarPlay invokes when the user taps the button. You communicate the button’s purpose using a title and a text style that the button applies to the title.

## Topics

### Creating a Text Button

init(title: String, textStyle: CPTextButtonStyle, handler: ((CPTextButton) -> Void)?)

Creates a button that displays a title in a specific style.

### Managing the Title

var title: String

The text the button displays.

### Managing the Button Style

var textStyle: CPTextButtonStyle

The text style the button applies to its title.

enum CPTextButtonStyle

The styles a button can apply to its title to communicate its action.

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

## See Also

### Location and Information

class CPPointOfInterestTemplate

A template that displays a map with selectable points of interest.

class CPInformationTemplate

A template that provides information for a point of interest, food order, parking location, or charging location.

Integrating CarPlay with your quick-ordering app

Configure your food-ordering app to work with CarPlay.

