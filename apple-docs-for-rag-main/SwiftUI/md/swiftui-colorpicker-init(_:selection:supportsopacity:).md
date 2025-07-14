

- SwiftUI
- ColorPicker
-  init(\_:selection:supportsOpacity:) 

Initializer

# init(\_:selection:supportsOpacity:)

Creates a color picker with a text label generated from a title string key.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
nonisolated
init(
    _ titleKey: LocalizedStringKey,
    selection: Binding,
    supportsOpacity: Bool = true
)
```

Available when `Label` is `Text`.

Show all declarations

## Parameters 

`titleKey`  

The key for the localized title of the picker.

`selection`  

A Binding to the variable that displays the selected `CGColor`.

`supportsOpacity`  

A Boolean value that indicates whether the color picker allows adjustments to the selected color’s opacity; the default is `true`.

## See Also

### Creating a color picker

init(selection:supportsOpacity:label:)

Creates an instance that selects a color.

