

- SwiftUI
- Picker
-  init(sources:selection:content:label:currentValueLabel:) 

Initializer

# init(sources:selection:content:label:currentValueLabel:)

Creates a picker that displays a custom label and current value label where applicable.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
init(
    sources: C,
    selection: KeyPath>,
    @ViewBuilder content: () -> Content,
    @ViewBuilder label: () -> Label,
    @ViewBuilder currentValueLabel: () -> some View
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

`currentValueLabel`  

A view that represents the current value of the picker.

## Discussion

If the wrapped values of the collection passed to `sources` are not all the same, some styles render the selection in a mixed state. The specific presentation depends on the style. For example, a Picker with a menu style uses dashes instead of checkmarks to indicate the selected values.

In the following example, a picker in a document inspector controls the thickness of borders for the currently selected shapes.

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
} currentValueLabel: {
     switch selectedObjectBorders.count {
        case 0: Text("None")
        case 1: Text(selectedObjectBorders[0].thickness.rawValue)
        default: Text("Multiple")
     }
} label: {
    Text("Border Thickness")
}
```

