

- SwiftUI
- Picker
-  init(\_:systemImage:selection:content:currentValueLabel:) 

Initializer

# init(\_:systemImage:selection:content:currentValueLabel:)

Creates a picker that accepts a custom current value label and generates its label from a localized string key and system image.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
init(
    _ titleKey: LocalizedStringKey,
    systemImage: String,
    selection: Binding,
    @ViewBuilder content: () -> Content,
    @ViewBuilder currentValueLabel: () -> some View
)
```

Available when `Label` is `Label`, `SelectionValue` conforms to `Hashable`, and `Content` conforms to `View`.

Show all declarations

## Parameters 

`titleKey`  

A localized string key that describes the purpose of selecting an option.

`systemImage`  

The name of the image resource to lookup.

`selection`  

A binding to a property that determines the currently-selected option.

`content`  

A view that contains the set of options.

`currentValueLabel`  

A view that represents the current value of the picker.

## Discussion

This initializer creates a Text view on your behalf, and treats the localized key similar to init(_:tableName:bundle:comment:). See Text for more information about localizing strings.

