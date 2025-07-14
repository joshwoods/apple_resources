

- CarPlay
-  CPInformationTemplate 

Class

# CPInformationTemplate

A template that provides information for a point of interest, food order, parking location, or charging location.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class CPInformationTemplate
```

## Overview

An information template displays a list of items, and up to three actions the user can perform.

You use an information template to display informative, actionable content to the user. For example, you might display a summary of the user’s food order, and provide actions to place or cancel the order.

When creating an information template, you populate the list with an array of CPInformationItem objects, and provide any contextual actions as an array of CPTextButton objects. The template then arranges the list’s items using your choice of layout — see CPInformationTemplateLayout for more information.

To display an information template, call your interface controller’s pushTemplate(_:animated:completion:) method to push it onto the navigation hierarchy, or presentTemplate(_:animated:completion:) to present it modally.

Note

You can’t use `CPInformationTemplate` in apps with the audio entitlement.

## Topics

### Creating an Information Template

init(title: String, layout: CPInformationTemplateLayout, items: [CPInformationItem], actions: [CPTextButton])

Creates an information template that displays the provided items using the chosen layout.

### Accessing the Layout

var layout: CPInformationTemplateLayout

The layout that the template uses to arrange its items.

enum CPInformationTemplateLayout

The layout that an information template uses to arrange its items.

### Managing the Title

var title: String

The template’s title.

### Managing the Items

var items: [CPInformationItem]

The items that the template displays.

class CPInformationItem

A data object that provides content for an information template.

class CPInformationRatingItem

A data object that provides rated content for an information template.

### Managing the Actions

var actions: [CPTextButton]

The actions that the template displays.

## Relationships

### Inherits From

- CPTemplate

### Conforms To

- CPBarButtonProviding
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Location and Information

class CPPointOfInterestTemplate

A template that displays a map with selectable points of interest.

class CPTextButton

A button that displays a stylized title.

Integrating CarPlay with your quick-ordering app

Configure your food-ordering app to work with CarPlay.

