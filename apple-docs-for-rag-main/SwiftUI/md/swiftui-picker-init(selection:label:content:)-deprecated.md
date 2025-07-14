

- SwiftUI
- Picker
-  init(selection:label:content:) Deprecated

Initializer

# init(selection:label:content:)

Creates a picker that displays a custom label.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 6.0–11.4Deprecated

``` source
nonisolated
init(
    selection: Binding,
    label: Label,
    @ViewBuilder content: () -> Content
)
```

Available when `Label` conforms to `View`, `SelectionValue` conforms to `Hashable`, and `Content` conforms to `View`.

Deprecated

Use init(selection:content:label:) instead.

## Parameters 

`selection`  

A binding to a property that determines the currently-selected option.

`label`  

A view that describes the purpose of selecting an option.

`content`  

A view that contains the set of options.

