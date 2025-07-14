

- RealityKit
- RealityView
-  lineLimit(\_:) 

Instance Method

# lineLimit(\_:)

Sets to a partial range the number of lines that text can occupy in this view.

RealityKitSwiftUIiOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
nonisolated
func lineLimit(_ limit: PartialRangeFrom) -> some View
```

## Parameters 

`limit`  

The line limit.

## Discussion

Use this modifier to specify a partial range of lines that a `Text` view or a vertical `TextField` can occupy. When the text of such views occupies less space than the provided limit, that view expands to occupy the minimum number of lines.

```
Form {
    TextField("Title", text: $model.title)
    TextField("Notes", text: $model.notes, axis: .vertical)
        .lineLimit(3...)
}
```

