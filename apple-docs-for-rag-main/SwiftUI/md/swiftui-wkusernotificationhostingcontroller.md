

- SwiftUI
-  WKUserNotificationHostingController 

Class

# WKUserNotificationHostingController

A WatchKit user notification interface controller that hosts a SwiftUI view hierarchy.

watchOS 6.0+

``` source
@MainActor @preconcurrency
class WKUserNotificationHostingController where Body : View
```

## Overview

A WKUserNotificationHostingController presents and manages your app’s notification interface using SwiftUI views. You must subclass WKUserNotificationHostingController and override the body property to provide the set of SwiftUI views you want to display. In the storyboard of your watch app, specify the name of your custom class for your dynamic interactive interface.

## Topics

### Creating a hosting controller object

init()

Creates a notification hosting controller object that you can use to implement your notification interfaces using SwiftUI views.

### Getting the root view

var body: Body

The root view of the view hierarchy to display for your notification interface.

### Configuring the notification

class var coalescedDescriptionFormat: String?

The format string to display when multiple notifications of the same type arrive simultaneously. If you specify a custom string, you can use the %d variable to reflect the number of notifications. If `nil` format will be the system default.

class var isInteractive: Bool

If the notification should accept user input.

class var sashColor: Color?

Color to use within the sash of the long look interface. If `nil` the sash will be the default system color.

class var subtitleColor: Color?

The color to apply to the subtitle text displayed in the short look interface. If `nil` the text will be the default system color.

class var titleColor: Color?

The color to apply to the text displayed in the sash. If `nil` the text will be the default system color.

class var wantsSashBlur: Bool

If the sash should include a blur over the background.

## Relationships

### Inherits From

- WKUserNotificationInterfaceController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Displaying SwiftUI views in WatchKit

class WKHostingController

A WatchKit interface controller that hosts a SwiftUI view hierarchy.

