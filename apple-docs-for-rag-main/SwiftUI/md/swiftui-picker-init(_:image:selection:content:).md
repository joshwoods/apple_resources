

- SwiftUI
- Picker
-  init(\_:image:selection:content:) 

Initializer

# init(\_:image:selection:content:)

Creates a picker that generates its label from a localized string key and image resource

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
init(
    _ titleKey: LocalizedStringKey,
    image: ImageResource,
    selection: Binding,
    @ViewBuilder content: () -> Content
)
```

Available when `Label` is `Label`, `SelectionValue` conforms to `Hashable`, and `Content` conforms to `View`.

Show all declarations

## Parameters 

`titleKey`  

A localized string key that describes the purpose of selecting an option.

`image`  

The name of the image resource to lookup.

`selection`  

A binding to a property that determines the currently-selected option.

`content`  

A view that contains the set of options.

## Discussion

This initializer creates a Text view on your behalf, and treats the localized key similar to init(_:tableName:bundle:comment:). See Text for more information about localizing strings.

## See Also

### Creating a picker with an image label

init(_:image:sources:selection:content:)

Creates a picker bound to a collection of bindings that generates its label from a string and image resource.

init(_:systemImage:selection:content:)

Creates a picker that generates its label from a localized string key and system image.

init(_:systemImage:sources:selection:content:)

Creates a picker bound to a collection of bindings that generates its label from a string.

