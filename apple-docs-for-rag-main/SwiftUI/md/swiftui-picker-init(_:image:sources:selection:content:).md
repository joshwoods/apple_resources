

- SwiftUI
- Picker
-  init(\_:image:sources:selection:content:) 

Initializer

# init(\_:image:sources:selection:content:)

Creates a picker bound to a collection of bindings that generates its label from a string and image resource.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
init(
    _ title: S,
    image: ImageResource,
    sources: C,
    selection: KeyPath>,
    @ViewBuilder content: () -> Content
) where C : RandomAccessCollection, S : StringProtocol, C.Element == Binding
```

Available when `Label` is `Label`, `SelectionValue` conforms to `Hashable`, and `Content` conforms to `View`.

Show all declarations

## Parameters 

`title`  

A string that describes the purpose of selecting an option.

`image`  

The name of the image resource to lookup.

`sources`  

A collection of values used as the source for displaying the Picker’s selection.

`selection`  

The key path of the values that determines the currently-selected options. When a user selects an option from the picker, the values at the key path of all items in the `sources` collection are updated with the selected option.

`content`  

A view that contains the set of options.

## Discussion

If the wrapped values of the collection passed to `sources` are not all the same, some styles render the selection in a mixed state. The specific presentation depends on the style. For example, a Picker with a menu style uses dashes instead of checkmarks to indicate the selected values.

In the following example, a picker in a document inspector controls the thickness of borders for the currently-selected shapes, which can be of any number.

```
enum Thickness: String, CaseIterable, Identifiable {
    case thin
    case regular
    case thick

    var id: String { rawValue }
}

struct Border {
    var color: Color
    var thickness: Thickness
}

@State private var selectedObjectBorders = [
    Border(color: .black, thickness: .thin),
    Border(color: .red, thickness: .thick)
]

Picker(
    "Border Thickness",
    sources: $selectedObjectBorders,
    selection: \.thickness
) {
    ForEach(Thickness.allCases) { thickness in
        Text(thickness.rawValue)
    }
}
```

## See Also

### Creating a picker with an image label

init(_:image:selection:content:)

Creates a picker that generates its label from a localized string key and image resource

init(_:systemImage:selection:content:)

Creates a picker that generates its label from a localized string key and system image.

init(_:systemImage:sources:selection:content:)

Creates a picker bound to a collection of bindings that generates its label from a string.

