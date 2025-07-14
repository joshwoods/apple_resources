

- SwiftUI
-  MenuButtonStyle Deprecated

Protocol

# MenuButtonStyle

A custom specification for the appearance and interaction of a menu button.

macOS 10.15–15.4Deprecated

``` source
protocol MenuButtonStyle
```

Deprecated

Use MenuStyle instead.

## Topics

### Supporting types

struct BorderlessButtonMenuButtonStyle

A menu button style which manifests as a borderless button with no visual embelishments.

struct BorderlessPullDownMenuButtonStyle

A menu button style which manifests as a borderless pull-down button.

struct DefaultMenuButtonStyle

The default menu button style.

struct PullDownMenuButtonStyle

A menu button style which manifests as a pull-down button.

## Relationships

### Conforming Types

- BorderlessButtonMenuButtonStyle
- BorderlessPullDownMenuButtonStyle
- DefaultMenuButtonStyle
- PullDownMenuButtonStyle

## See Also

### Styling a menu button

func menuButtonStyle&lt;S>(S) -> some View

Sets the style for menu buttons within this view.

Deprecated

