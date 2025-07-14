

- WidgetKit
-  ActivityPreviewViewKind 

Enumeration

# ActivityPreviewViewKind

Values that represent Live Activity presentations for use in Xcode previews.

iOS 16.2+iPadOS 16.2+Mac Catalyst 16.2+

``` source
@preconcurrency
enum ActivityPreviewViewKind
```

## Topics

### Live Activity preview types

case content

The Live Activity presentation that appears on the Lock Screen and as a banner on devices that don’t support the Dynamic Island.

case dynamicIsland(ActivityPreviewViewKind.DynamicIslandPreviewViewState)

The Live Activity presentation that appears in the Dynamic Island.

enum DynamicIslandPreviewViewState

Values that represent the different presentations of a Live Activity in the Dynamic Island for use in Xcode previews.

## Relationships

### Conforms To

- Sendable

## See Also

### Live Activities

struct ActivityConfiguration

An object that describes the content of a Live Activity.

struct DynamicIsland

The layout and configuration for a Live Activity that appears in the Dynamic Island.

let NSUserActivityTypeLiveActivity: String

A string that the system passes to the app on launch from a Live Activity that doesn’t provide a URL.

enum ActivityFamily

A family that defines the Live Activity’s size.

