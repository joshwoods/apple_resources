

- WidgetKit
-  ActivityFamily 

Enumeration

# ActivityFamily

A family that defines the Live Activity’s size.

iOS 18.0+iPadOS 18.0+

``` source
enum ActivityFamily
```

## Overview

Live Activities support one or more sizes, giving you the flexibility to configure them for different devices. A Live Activity renders for a specific family, depending on both the device and the location in which it’s displayed.

A Live Activity initiated on one device can be sent to a remote device that renders the Live Activity at a different family size. For example, if your Live Activity is running on an iOS or iPadOS device, it natively renders with an ActivityFamily.medium family. If you want to opt in to customize the rendering for a Live Activity for the watchOS Smart Stack, use the ActivityFamily.small family modifier.

When you define your Live Activity’s configuration, specify the sizes your Live Activity supports using the supplementalActivityFamilies(_:) property modifier.

When you render the content of the Live Activity, use activityFamily to read the current family and lay out your content appropriately. The code below uses supplementalActivityFamilies(_:) to specify the size of the Live Activity for devices on iOS and watchOS.

```
// A RideSharingActivity that supports the watchOS Smart Stack and the iOS Lock Screen.
struct RideSharingActivity: Widget {
   var body: some WidgetConfiguration {
       ActivityConfiguration(for: RideAttributes.self) { context in
           RideSharingView(context: context)
       } dynamicIsland: { context in
           DynamicIsland {
               DynamicIslandExpandedRegion(.bottom) {
                   RideShareDetails()
               }
           } compactLeading: {
               AppLogo()
           } compactTrailing: {
               ETAView()
           } minimal: {
               ETAView()
           }
       }
       .supplementalActivityFamilies([.small, .medium])
   }
}
```

## Topics

### Accessing system families

case small

A size family of a Live Activity on watchOS.

case medium

A size family of a Live Activity on iOS.

### Environment keys

struct SupportedActivityFamiliesEnvironmentKey

An environment key for the size of a rendered Live Activity.

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- RawRepresentable

## See Also

### Live Activities

struct ActivityConfiguration

An object that describes the content of a Live Activity.

struct DynamicIsland

The layout and configuration for a Live Activity that appears in the Dynamic Island.

let NSUserActivityTypeLiveActivity: String

A string that the system passes to the app on launch from a Live Activity that doesn’t provide a URL.

enum ActivityPreviewViewKind

Values that represent Live Activity presentations for use in Xcode previews.

