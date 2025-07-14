

- WidgetKit
-  WidgetLocation 

Structure

# WidgetLocation

Values that indicate different widget locations.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
struct WidgetLocation
```

## Mentioned in 

Preparing widgets for additional platforms, contexts, and appearances

## Topics

### Specifying a location style

static let iPhoneWidgetsOnMac: WidgetLocation

The widget originates from another device and appears on the Mac.

static let homeScreen: WidgetLocation

The widget appears on the Home Screen or in Today View.

static let lockScreen: WidgetLocation

The widget appears on the Lock Screen.

static let standBy: WidgetLocation

The widget appears in StandBy.

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Presentation

Creating views for widgets, Live Activities, and watch complications

Implement glanceable views with WidgetKit and SwiftUI.

Preparing widgets for additional platforms, contexts, and appearances

Create widgets that support additional platforms and adapt to their context.

SwiftUI views for widgets

Present your app’s content in widgets with SwiftUI views.

Introducing SwiftUI

SwiftUI is a modern way to declare user interfaces for any Apple platform. Create beautiful, dynamic apps faster than ever before.

struct AccessoryWidgetBackground

An adaptive background view that provides a standard appearance based on the the widget’s environment.

