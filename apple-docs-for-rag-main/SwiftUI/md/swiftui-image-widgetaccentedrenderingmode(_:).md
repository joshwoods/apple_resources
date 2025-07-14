

- SwiftUI
- Image
-  widgetAccentedRenderingMode(\_:) 

Instance Method

# widgetAccentedRenderingMode(\_:)

Specifies the how to render an `Image` when using the `WidgetKit/WidgetRenderingMode/accented` mode.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+watchOS 11.0+

``` source
func widgetAccentedRenderingMode(_ renderingMode: WidgetAccentedRenderingMode?) -> some View
```

## Parameters 

`renderingMode`  

A constant describing how the `Image` should be rendered.

## Discussion

```
var body: some View {
    VStack {
        Image("cat_full")
            .resizable()
            .widgetAccentedRenderingMode(.fullColor)
    }
}
```

Important

If the `Image` is a subview for a group that has `widgetAccentable(true)` applied, this modifier may conflict.

