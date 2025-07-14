

- SwiftUI
- ControlGroupStyle
-  palette 

Type Property

# palette

A control group style that presents its content as a palette.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
static var palette: PaletteControlGroupStyle { get }
```

Available when `Self` is `PaletteControlGroupStyle`.

## Discussion

Note

When used outside of menus, this style is rendered as a segmented control.

Use this style to render a multi-select or a stateless palette. The following example creates a control group that contains both type of shelves:

```
Menu {
    // A multi select palette
    ControlGroup {
        ForEach(ColorTags.allCases) { colorTag in
            Toggle(isOn: $selectedColorTags[colorTag]) {
                Label(colorTag.name, systemImage: "circle")
            }
            .tint(colorTag.color)
        }
    }
    .controlGroupStyle(.palette)
    .paletteSelectionEffect(.symbolVariant(.fill))

    // A momentary / stateless palette
    ControlGroup {
        ForEach(Emotes.allCases) { emote in
            Button {
                sendEmote(emote)
            } label: {
                Label(emote.name, systemImage: emote.systemImage)
            }
        }
    }
    .controlGroupStyle(.palette)
}
```

To apply this style to a control group, or to a view that contains control groups, use the controlGroupStyle(_:) modifier.

## See Also

### Getting built-in control group styles

static var automatic: AutomaticControlGroupStyle

The default control group style.

static var compactMenu: CompactMenuControlGroupStyle

A control group style that presents its content as a compact menu when the user presses the control, or as a submenu when nested within a larger menu.

static var menu: MenuControlGroupStyle

A control group style that presents its content as a menu when the user presses the control, or as a submenu when nested within a larger menu.

static var navigation: NavigationControlGroupStyle

The navigation control group style.

