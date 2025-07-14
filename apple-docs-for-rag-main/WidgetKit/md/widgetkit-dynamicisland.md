

- WidgetKit
-  DynamicIsland 

Structure

# DynamicIsland

The layout and configuration for a Live Activity that appears in the Dynamic Island.

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+

``` source
struct DynamicIsland
```

## Topics

### Creating the view for the Dynamic Island

init&lt;Expanded, CompactLeading, CompactTrailing, Minimal>(expanded: () -> DynamicIslandExpandedContent&lt;Expanded>, compactLeading: () -> CompactLeading, compactTrailing: () -> CompactTrailing, minimal: () -> Minimal)

Creates a configuration object with views that appear in the Dynamic Island.

struct DynamicIslandExpandedRegion

A structure that defines and positions the content of an expanded Live Activity in the Dynamic Island.

### Deep linking

func widgetURL(URL?) -> DynamicIsland

Sets the URL that opens the corresponding app of a Live Activity when a user taps on the Live Activity.

### Setting a tint color

func keylineTint(Color?) -> DynamicIsland

Applies a subtle tint color to the surrounding border of a Live Activity that appears in the Dynamic Island.

### Specifying content margins

func contentMargins(Edge.Set, Double, for: DynamicIslandMode) -> DynamicIsland

Overrides default content margins for the provided content modes in the Dynamic Island.

struct DynamicIslandMode

A structure that offers values that describe the content mode for a Live Activity.

## See Also

### Live Activities

struct ActivityConfiguration

An object that describes the content of a Live Activity.

let NSUserActivityTypeLiveActivity: String

A string that the system passes to the app on launch from a Live Activity that doesn’t provide a URL.

enum ActivityPreviewViewKind

Values that represent Live Activity presentations for use in Xcode previews.

enum ActivityFamily

A family that defines the Live Activity’s size.

