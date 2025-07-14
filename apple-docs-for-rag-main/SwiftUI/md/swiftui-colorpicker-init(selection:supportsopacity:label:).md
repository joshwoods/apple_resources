

- SwiftUI
- ColorPicker
-  init(selection:supportsOpacity:label:) 

Initializer

# init(selection:supportsOpacity:label:)

Creates an instance that selects a color.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
init(
    selection: Binding,
    supportsOpacity: Bool = true,
    @ViewBuilder label: () -> Label
)
```

Show all declarations

## Parameters 

`selection`  

A Binding to the variable that displays the selected `CGColor`.

`supportsOpacity`  

A Boolean value that indicates whether the color picker allows adjusting the selected color’s opacity; the default is `true`.

`label`  

A view that describes the use of the selected color. The system color picker UI sets it’s title using the text from this view.

## See Also

### Creating a color picker

init(_:selection:supportsOpacity:)

Creates a color picker with a text label generated from a title string key.

