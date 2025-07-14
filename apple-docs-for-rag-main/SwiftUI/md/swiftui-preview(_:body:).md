

- SwiftUI
-  Preview(\_:body:) 

Macro

# Preview(\_:body:)

Creates a preview of a SwiftUI view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@freestanding(declaration)
macro Preview(
    _ name: String? = nil,
    @ViewBuilder body: @escaping @MainActor () -> any View
)
```

## Parameters 

`name`  

An optional display name for the preview. If you don’t specify a name, the canvas labels the preview using the line number where the preview appears in source.

`body`  

A ViewBuilder that produces a SwiftUI view to preview. You typically specify one of your app’s custom views and optionally any inputs, model data, modifiers, and enclosing views that the custom view needs for normal operation.

## Overview

Use this macro to display a SwiftUI preview in the canvas. You typically specify at least one preview macro for every View that your app defines to help you develop, test, and debug the view:

```
struct ContentView: View {
    var body: some View {
        // ...
    }
}

#Preview {
    ContentView()
}
```

If you include more than one preview in a source file, the canvas provides controls that enable you to select which to display when that source file is active. The canvas labels the different previews with the line number where the preview appears in source. To better identify the previews in the canvas, you can give them names. For example if your `ContentView` takes a Boolean input, you can create named previews for each input state:

```
#Preview("Input true") {
    ContentView(someInput: true)
}

#Preview("Input false") {
    ContentView(someInput: false)
}
```

Inside the preview, you can provide different inputs, model data, and other infrastructure that the view needs for normal operation. For example, you can present a custom view as the sidebar inside a NavigationSplitView if that’s how your app uses the view.

Other preview macros provide different customization options. For example, if you need to modify the appearance of a preview using one or more PreviewTrait, instances, use the Preview(_:traits:_:body:) macro.

## See Also

### Creating a preview

macro Preview(String?, traits: PreviewTrait&lt;Preview.ViewTraits>, PreviewTrait&lt;Preview.ViewTraits>..., body: () -> any View)

Creates a preview of a SwiftUI view using the specified traits.

macro Preview(String?, traits: PreviewTrait&lt;Preview.ViewTraits>..., body: () -> any View, cameras: () -> [PreviewCamera])

Creates a preview of a SwiftUI view using the specified traits and custom viewpoints.

