

- SwiftUI
- LabelStyle
-  iconOnly 

Type Property

# iconOnly

A label style that only displays the icon of the label.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@MainActor @preconcurrency
static var iconOnly: IconOnlyLabelStyle { get }
```

Available when `Self` is `IconOnlyLabelStyle`.

## Discussion

The title of the label is still used for non-visual descriptions, such as VoiceOver.

## See Also

### Getting built-in label styles

static var automatic: DefaultLabelStyle

A label style that resolves its appearance automatically based on the current context.

static var titleAndIcon: TitleAndIconLabelStyle

A label style that shows both the title and icon of the label using a system-standard layout.

static var titleOnly: TitleOnlyLabelStyle

A label style that only displays the title of the label.

