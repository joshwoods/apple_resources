

- SwiftUI
- Picker
-  init(\_:systemImage:sources:selection:content:currentValueLabel:) 

Initializer

# init(\_:systemImage:sources:selection:content:currentValueLabel:)

Creates a picker bound to a collection of bindings that accepts a custom current value label and generates its label from a string.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
init(
    _ title: S,
    systemImage: String,
    sources: C,
    selection: KeyPath>,
    @ViewBuilder content: () -> Content,
    @ViewBuilder currentValueLabel: () -> some View
) where C : RandomAccessCollection, S : StringProtocol, C.Element == Binding
```

Available when `Label` is `Label`, `SelectionValue` conforms to `Hashable`, and `Content` conforms to `View`.

Show all declarations

## Parameters 

`title`  

A string that describes the purpose of selecting an option.

`systemImage`  

The name of the image resource to lookup.

`sources`  

A collection of values used as the source for displaying the Picker’s selection.

`selection`  

The key path of the values that determines the currently-selected options. When a user selects an option from the picker, the values at the key path of all items in the `sources` collection are updated with the selected option.

`content`  

A view that contains the set of options.

`currentValueLabel`  

A view that represents the current value of the picker.

