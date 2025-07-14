

- SwiftUI
- Picker
-  init(sources:selection:content:label:) 

Initializer

# init(sources:selection:content:label:)

Creates a picker that displays a custom label.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    sources: C,
    selection: KeyPath>,
    @ViewBuilder content: () -> Content,
    @ViewBuilder label: () -> Label
) where C : RandomAccessCollection
```

Available when `Label` conforms to `View`, `SelectionValue` conforms to `Hashable`, and `Content` conforms to `View`.

## Parameters 

`sources`  

A collection of values used as the source for displaying the Picker’s selection.

`selection`  

The key path of the values that determines the currently-selected options. When a user selects an option from the picker, the values at the key path of all items in the `sources` collection are updated with the selected option.

`content`  

A view that contains the set of options.

`label`  

A view that describes the purpose of selecting an option.

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
    sources: $selectedObjectBorders,
    selection: \.thickness
) {
    ForEach(Thickness.allCases) { thickness in
        Text(thickness.rawValue)
    }
} label: {
    Text("Border Thickness")
}
```

## See Also

### Creating a picker for a collection

init(_:sources:selection:content:)

Creates a picker bound to a collection of bindings that generates its label from a string.

