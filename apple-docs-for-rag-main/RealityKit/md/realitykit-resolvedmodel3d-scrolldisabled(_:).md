

- RealityKit
- ResolvedModel3D
-  scrollDisabled(\_:) 

Instance Method

# scrollDisabled(\_:)

Disables or enables scrolling in scrollable views.

RealityKitSwiftUIiOS 16.0+iPadOS 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
nonisolated
func scrollDisabled(_ disabled: Bool) -> some View
```

## Parameters 

`disabled`  

A Boolean that indicates whether scrolling is disabled.

## Discussion

Use this modifier to control whether a `ScrollView` can scroll:

```
@State private var isScrollDisabled = false

var body: some View {
    ScrollView {
        VStack {
            Toggle("Disable", isOn: $isScrollDisabled)
            MyContent()
        }
    }
    .scrollDisabled(isScrollDisabled)
}
```

SwiftUI passes the disabled property through the environment, which means you can use this modifier to disable scrolling for all scroll views within a view hierarchy. In the following example, the modifier affects both scroll views:

```
 ScrollView {
     ForEach(rows) { row in
         ScrollView(.horizontal) {
             RowContent(row)
         }
     }
 }
 .scrollDisabled(true)
```

You can also use this modifier to disable scrolling for other kinds of scrollable views, like a `List` or a `TextEditor`.

