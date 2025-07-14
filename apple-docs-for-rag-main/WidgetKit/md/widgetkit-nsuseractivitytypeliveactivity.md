

- WidgetKit
-  NSUserActivityTypeLiveActivity 

Global Variable

# NSUserActivityTypeLiveActivity

A string that the system passes to the app on launch from a Live Activity that doesn’t provide a URL.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+watchOS 9.0+

``` source
let NSUserActivityTypeLiveActivity: String
```

## Discussion

In many cases, you use widgetURL(_:) to allow users to tap a Live Activity and open a screen in the app with functionality that best fits the Live Activity. If you don’t use the `widgetURL(_:)` modifier to provide a URL, the system launches your app and passes `NSUserActivityTypeLiveActivity` as the activityType of NSUserActivity upon launch. Check for this value on launch to open a screen in your app that fits the context of the active Live Activity.

## See Also

### Live Activities

struct ActivityConfiguration

An object that describes the content of a Live Activity.

struct DynamicIsland

The layout and configuration for a Live Activity that appears in the Dynamic Island.

enum ActivityPreviewViewKind

Values that represent Live Activity presentations for use in Xcode previews.

enum ActivityFamily

A family that defines the Live Activity’s size.

