

- WidgetKit
-  Preparing widgets for additional platforms, contexts, and appearances 

Article

# Preparing widgets for additional platforms, contexts, and appearances

Create widgets that support additional platforms and adapt to their context.

## Overview

Widgets change their appearance to best fit their context. For example, widgets on the Home Screen, Today View, or the macOS Notification Center use full colors and rich images to represent your brand and encourage people to feature your widget on their devices. In contrast, Lock Screen widgets and WidgetKit complications use more restrained colors because they’re smaller, always visible, and support tinted modes for each platform. Since all widgets appear in more than one context, make sure your widgets and their SwiftUI views support all applicable rendering modes.

WidgetKit uses three different rendering modes:

vibrant  
Desaturates text, images, and gauges into monochrome and creates a vibrant effect by coloring your content appropriately for the Lock Screen background or the macOS desktop. Note that people can also color the Lock Screen to a colored tint and WidgetKit uses a red tint for widgets that appear on iPhone in StandBy in low-light conditions.

fullColor  
Doesn’t change the color of your complication’s views in this rendering mode. Use gradients and full-color images, text, and gauges.

accented  
Renders complications in the accented rendering mode when people customize their device to use a tint color or choose certain watch faces. The system divides the widget’s view hierarchy into an accent group and a default group, and then applies a solid color to each group. Use the widgetAccentable(_:) view modifier to group views into the accented group. Note that this rendering mode isn’t available in macOS.

The following table shows the rendering modes for each widget you need to support:

| Widget size | fullColor | accented | vibrant |
|----|----|----|----|
| WidgetFamily.systemSmall | Yes | Yes | Yes |
| WidgetFamily.systemMedium | Yes | Yes | Yes |
| WidgetFamily.systemLarge | Yes | Yes | Yes |
| WidgetFamily.systemExtraLarge | Yes | Yes | Yes |
| WidgetFamily.accessoryCircular | No | Yes | Yes |
| WidgetFamily.accessoryCorner | No | Yes | Yes |
| WidgetFamily.accessoryRectangular | Yes | Yes | Yes |
| WidgetFamily.accessoryInline | No | Yes | Yes |

Note

For design guidance, see Human Interface Guidelines > Complications and Human Interface Guidelines > Widgets.

In your code, read the widgetRenderingMode environment variable to create SwiftUI views for each applicable rendering mode, as shown in the following example:

```
var body: some View {
   ZStack {
       switch renderingMode {
       case .fullColor:
           // Create views for full-color widgets and watch complications.
       case .accented:
           // Create views and group applicable views in the accented group.
           VStack {
               // ...
           }
           .widgetAccentable()
           // Additional views that you don't group in the accented group.
       case .vibrant:
           // Create views for Lock Screen widgets on iPhone and iPad, and for the receded appearance on the Mac desktop.
   }
}
```

### Support Always On

If you create accessory widgets and WidgetKit complications, make sure to use SwiftUI’s isLuminanceReduced environment variable to detect Always On and color your views to look great with reduced luminance. For design guidance, see Human Interface Guidelines > Always On and Human Interface Guidelines > Widgets.

### Update your small widget to support StandBy

On iPhone in StandBy, the Lock Screen shows two widgets side by side on a dark background. WidgetKit uses your WidgetFamily.systemSmall widget and scales it to fit one half of the screen. To support this appearance:

- Make the widget’s background removable with a container background, as described below.

- Update the widget’s layout to take advantage of the larger appearance and smaller content margins and to make the widget easier to read from a larger distance.

### Display the correct widget background for each context

Widgets appear differently based on their context, including their background view, for example:

- In the vibrant appearance, the system removes the background of your widget or renders it with semi-translucent appearance.

- In StandBy on iPhone, the system removes the background of your widget.

- On the Mac desktop, the system removes the background of your widget.

To make sure your widget appears correctly, mark your background views as removable for the following widget sizes:

- WidgetFamily.systemSmall

- WidgetFamily.systemMedium

- WidgetFamily.systemLarge

- WidgetFamily.systemExtraLarge

- WidgetFamily.accessoryRectangular

Important

If a widget doesn’t support removable background views or doesn’t explicitly mark a background as nonremovable, the system displays a warning message that overlays the widget during development with Xcode.

To mark your background views as removable:

1.  Add the containerBackground(_:for:) modifier to your background views to define the background appearance of your widget and tell WidgetKit that it can remove the view where applicable.

2.  Move code that declares any background color or views inside the `containerBackground(for:)` view modifier and pass widget to it. This makes sure WidgetKit automatically removes the background as needed.

The following code snippet from the Emoji Rangers: Supporting Live Activities, interactivity, and animations sample code project defines a `gameBackground` color for the widget’s container background to make sure WidgetKit renders it with or without the background color as applicable.

```
var body: some View {
    switch family {
    // Logic for additional widget sizes.
    case .accessoryRectangular:
        HStack(alignment: .center, spacing: 0) {
            VStack(alignment: .leading) {
                Text(entry.hero.name)
                    .font(.headline)
                    .widgetAccentable()
                Text("Level \(entry.hero.level)")
                Text(entry.hero.fullHealthDate, style: .timer)
            }.frame(maxWidth: .infinity, alignment: .leading)
            Avatar(hero: entry.hero, includeBackground: false)
        }
        .containerBackground(for: .widget) {
            Color.gameBackground
        }
       // Logic for additional widget sizes.
}
```

Marking background views as removable by defining a background container allows you to use the same layout and views for your widget across contexts. For example, if you support the rectangular accessory widget size as shown in the code snippet above, WidgetKit renders it with a rich, full-color background in the Smart Stack on Apple Watch and without a background as a watch complication or on the Lock Screen of iPhone and iPad.

Note

On Apple Watch, rectangular widgets in the Smart Stack use a default dark material background. By adding a container background, the widget renders with a background that visually ties it to your app and makes it more recognizable to people.

To detect whether a widget appears with or without a background, use the showsWidgetContainerBackground environment variable.

### Explicitly opt out of background removal

Some widgets don’t have distinct foreground content, and background removal can negatively impact their functionality. For example, a widget might display a photo or map that takes up the entirety of the widget’s bounds. Removing the photo or map removes the functionality of the widget. If this case applies to your widget, set the containerBackgroundRemovable(_:) modifier to `false` for your widget configuration.

Important

Marking a background as nonremovable excludes your widget from the widget gallery in contexts that require a removable background; for example, on the iPad Lock Screen and in StandBy.

### Set the background color of accessory widgets

Depending on your accessory widget or complication, you may need to set a consistent background for your accessory widget. Use AccessoryWidgetBackground to draw a consistent background for your widget, as shown in the following example. It creates a view that’s similar to the circular Lock Screen widget that the Calendar app offers:

```
ZStack {
     AccessoryWidgetBackground()
     VStack {
        Text(“MON”)
        Text(“6”)
         .font(.title)
    }
}
```

### Indicate that a widget might not fit a specific context

By default, the system suggests widgets in many contexts, and people can choose widgets in the widget gallery to personalize their system experience. However, a widget might not a good fit for a specific context. For example, a widget that relies on high-resolution photos and background colors for its functionality may not work well on the Lock Screen, where the system applies a vibrant treatment to the widget. To indicate that a widget doesn’t work well in a specific context, use disfavoredLocations(_:for:) and provide the applicable WidgetLocation. As a result, the widget appears in the widget gallery’s “Other” section for the disfavored location.

### Verify font sizes in macOS

When people place an iPhone widget on the Mac desktop, the system renders it using iOS font metrics. However, a native Mac app’s widgets use macOS font sizing. If you’re sharing code across your iOS and macOS targets in your Xcode project, make sure to verify font sizing in macOS and adjust it for macOS as needed.

## See Also

### Presentation

Creating views for widgets, Live Activities, and watch complications

Implement glanceable views with WidgetKit and SwiftUI.

SwiftUI views for widgets

Present your app’s content in widgets with SwiftUI views.

Introducing SwiftUI

SwiftUI is a modern way to declare user interfaces for any Apple platform. Create beautiful, dynamic apps faster than ever before.

struct AccessoryWidgetBackground

An adaptive background view that provides a standard appearance based on the the widget’s environment.

struct WidgetLocation

Values that indicate different widget locations.

