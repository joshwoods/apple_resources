

- Notification Center
-  NCWidgetController Deprecated

Class

# NCWidgetController

An object used to specify whether a Today widget has content to display.

iOS 8.0–14.0DeprecatediPadOS 8.0–14.0DeprecatedMac Catalyst 8.0–14.0DeprecatedmacOS 10.10–11.0Deprecated

``` source
class NCWidgetController
```

Deprecated

Use WidgetKit instead.

## Overview

The `NCWidgetController` class defines an object that both a Today widget and the containing app that delivers the widget can use to specify whether the widget has content to display. Because this class helps a widget and its containing app coordinate the display of the widget’s content, a widget that doesn’t communicate with its containing app is unlikely to use this class.

Typically, a widget appears in the Today view when it has content to display. If a currently running widget no longer has content to display, it can get a widget controller and set the flag in the setHasContent(_:forWidgetWithBundleIdentifier:) method to `false`. If the containing app later determines that there is content this widget should display, the app can get a widget controller and update the flag, even while the widget isn’t running.

The `NCWidgetController` class should not be subclassed.

## Topics

### Getting a Widget Controller

class func widgetController() -> Self

Returns a widget controller used to specify whether a widget has content to display.

### Specifying the Presence of Content

func setHasContent(Bool, forWidgetWithBundleIdentifier: String)

Sets whether the specified widget has content to display.

### Type Methods

class func `default`() -> NCWidgetController

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

### Core Widget

protocol NCWidgetProviding

The interface for customizing the appearance and behavior of a Today widget.

Deprecated

