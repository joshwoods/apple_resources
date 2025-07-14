

- SwiftUI
- ToggleStyle
-  automatic 

Type Property

# automatic

The default toggle style.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@MainActor @preconcurrency
static var automatic: DefaultToggleStyle { get }
```

Available when `Self` is `DefaultToggleStyle`.

## Discussion

Use this ToggleStyle to let SwiftUI pick a suitable style for the current platform and context. Toggles use the `automatic` style by default, but you might need to set it explicitly using the toggleStyle(_:) modifier to override another style in the environment. For example, you can request automatic styling for a toggle in an HStack that’s otherwise configured to use the button style:

```
HStack {
    Toggle(isOn: $isShuffling) {
        Label("Shuffle", systemImage: "shuffle")
    }
    Toggle(isOn: $isRepeating) {
        Label("Repeat", systemImage: "repeat")
    }

    Divider()

    Toggle("Enhance Sound", isOn: $isEnhanced)
        .toggleStyle(.automatic) // Set the style automatically here.
}
.toggleStyle(.button) // Use button style for toggles in the stack.
```

### Platform defaults

The `automatic` style produces an appearance that varies by platform, using the following styles in most contexts:

| Platform | Default style |
|----|----|
| iOS, iPadOS | switch |
| macOS | checkbox |
| tvOS | switch |
| watchOS | switch |

The default style for tvOS behaves like a button. However, unlike the switch style that’s on other platforms, the tvOS toggle takes as much horizontal space as its parent offers, and displays both the toggle’s label and a text field that indicates the toggle’s state. You typically collect tvOS toggles into a List:

```
List {
    Toggle("Show Lyrics", isOn: $isShowingLyrics)
    Toggle("Shuffle", isOn: $isShuffling)
    Toggle("Repeat", isOn: $isRepeating)
}
```

### Contextual defaults

A toggle’s automatic appearance varies in certain contexts:

- A toggle that appears as part of the content that you provide to one of the toolbar modifiers, like toolbar(content:), uses the button style by default.

- A toggle in a Menu uses a style that you can’t create explicitly:

  ```
  Menu("Playback") {
      Toggle("Show Lyrics", isOn: $isShowingLyrics)
      Toggle("Shuffle", isOn: $isShuffling)
      Toggle("Repeat", isOn: $isRepeating)
  }
  ```

  SwiftUI shows the toggle’s label with a checkmark that appears only in the `on` state:

  | Platform | Appearance |
  |----|----|
  | iOS, iPadOS |  |
  | macOS |  |

## See Also

### Getting built-in toggle styles

static var button: ButtonToggleStyle

A toggle style that displays as a button with its label as the title.

static var checkbox: CheckboxToggleStyle

A toggle style that displays a checkbox followed by its label.

static var `switch`: SwitchToggleStyle

A toggle style that displays a leading label and a trailing switch.

