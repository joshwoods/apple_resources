

- SwiftUI
- WindowGroup
-  init(id:for:content:defaultValue:) 

Initializer

# init(id:for:content:defaultValue:)

Creates a data-presenting window group with an identifier and a default value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
nonisolated
init(
    id: String,
    for type: D.Type = D.self,
    @ViewBuilder content: @escaping (Binding) -> C,
    defaultValue: @escaping () -> D
) where Content == PresentedWindowContent, D : Decodable, D : Encodable, D : Hashable, C : View
```

Available when `Content` conforms to `View`.

## Parameters 

`id`  

A string that uniquely identifies the window group. Identifiers must be unique among the window groups in your app.

`type`  

The type of presented data this window group accepts.

`content`  

A closure that creates the content for each instance of the group. The closure receives a binding to the value that you pass into the openWindow action when you open the window. SwiftUI automatically persists and restores the value of this binding as part of the state restoration process.

`defaultValue`  

A closure that returns a default value to present. SwiftUI calls this closure when it has no data to provide, like when someone opens a new window from the File \> New Window menu item.

## Discussion

The window group uses the given view as a template to form the content of each window in the group.

SwiftUI creates a window from the group when you present a value of the specified type using the openWindow action.

## See Also

### Identifying a window group that has default data

init(_:id:for:content:defaultValue:)

Creates a data-presenting window group with a text view title, an identifier, and a default value.

