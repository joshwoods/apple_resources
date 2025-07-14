

- CarPlay
-  CPDashboardController 

Class

# CPDashboardController

A controller that provides shortcut buttons for the CarPlay Dashboard.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+

``` source
class CPDashboardController
```

## Overview

A dashboard controller manages up to two shortcut buttons that CarPlay displays in the dashboard when there’s no active navigation session. You don’t create the dashboard controller. Instead, CarPlay creates one for you and passes it to the delegate of CPTemplateApplicationDashboardScene when it connects the dashboard scene.

After receiving the controller, set shortcutButtons to an array that contains a maximum of two shortcut buttons. CarPlay manages hiding or showing the buttons on the dashboard at the appropriate times.

## Topics

### Providing Dashboard Buttons

var shortcutButtons: [CPDashboardButton]

An array of shortcut buttons to display on the CarPlay Dashboard.

class CPDashboardButton

A shortcut button for placement on the CarPlay Dashboard.

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

### Accessing the Dashboard Controller

var dashboardController: CPDashboardController

The controller that manages the dashboard scene’s shortcut buttons.

