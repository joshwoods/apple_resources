

- SwiftUI
-  WKHostingController 

Class

# WKHostingController

A WatchKit interface controller that hosts a SwiftUI view hierarchy.

watchOS 6.0+

``` source
@MainActor @preconcurrency
class WKHostingController where Body : View
```

## Overview

A WKHostingController presents and manages your app’s main interface using SwiftUI views. You must subclass WKHostingController and override the body property to provide the set of SwiftUI views you want to display. Display the content of your hosting controller as you would any other WKInterfaceController object. For example, you can include it as one of your app’s root interface controllers, or present it modally.

## Topics

### Creating a hosting controller object

init()

Creates a hosting controller object that you can use to implement your app’s main interface using SwiftUI views

### Getting the root view

var body: Body

The root view of the view hierarchy to display for your interface controller.

### Updating the root view

func updateBodyIfNeeded()

Updates the interface controller’s set of views immediately, if updates are pending.

func setNeedsBodyUpdate()

Invalidates the current SwiftUI views and triggers an update during the next cycle.

## Relationships

### Inherits From

- WKInterfaceController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Displaying SwiftUI views in WatchKit

class WKUserNotificationHostingController

A WatchKit user notification interface controller that hosts a SwiftUI view hierarchy.

