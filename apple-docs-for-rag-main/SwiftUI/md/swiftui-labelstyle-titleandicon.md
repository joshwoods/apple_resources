

- SwiftUI
- LabelStyle
-  titleAndIcon 

Type Property

# titleAndIcon

A label style that shows both the title and icon of the label using a system-standard layout.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+tvOS 14.5+visionOS 1.0+watchOS 7.4+

``` source
@MainActor @preconcurrency
static var titleAndIcon: TitleAndIconLabelStyle { get }
```

Available when `Self` is `TitleAndIconLabelStyle`.

## Discussion

In most cases, labels show both their title and icon by default. However, some containers might apply a different default label style to their content, such as only showing icons within toolbars on macOS and iOS. To opt in to showing both the title and the icon, you can apply the title and icon label style:

```
Label("Lightning", systemImage: "bolt.fill")
    .labelStyle(.titleAndIcon)
```

To apply the title and icon style to a group of labels, apply the style to the view hierarchy that contains the labels:

```
VStack {
    Label("Rain", systemImage: "cloud.rain")
    Label("Snow", systemImage: "snow")
    Label("Sun", systemImage: "sun.max")
}
.labelStyle(.titleAndIcon)
```

The relative layout of the title and icon is dependent on the context it is displayed in. In most cases, however, the label is arranged horizontally with the icon leading.

## See Also

### Getting built-in label styles

static var automatic: DefaultLabelStyle

A label style that resolves its appearance automatically based on the current context.

static var iconOnly: IconOnlyLabelStyle

A label style that only displays the icon of the label.

static var titleOnly: TitleOnlyLabelStyle

A label style that only displays the title of the label.

