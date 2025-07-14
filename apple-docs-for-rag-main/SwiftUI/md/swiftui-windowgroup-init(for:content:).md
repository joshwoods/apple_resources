

- SwiftUI
- WindowGroup
-  init(for:content:) 

Initializer

# init(for:content:)

Creates a data-presenting window group.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
nonisolated
init(
    for type: D.Type,
    @ViewBuilder content: @escaping (Binding) -> C
) where Content == PresentedWindowContent, D : Decodable, D : Encodable, D : Hashable, C : View
```

Available when `Content` conforms to `View`.

## Parameters 

`type`  

The type of presented data this window group accepts.

`content`  

A closure that creates the content for each instance of the group. The closure receives a binding to the value that you pass into the openWindow action when you open the window. SwiftUI automatically persists and restores the value of this binding as part of the state restoration process.

## Discussion

The window group uses the given view as a template to form the content of each window in the group.

SwiftUI creates a window from the group when you present a value of the specified type using the openWindow action.

## See Also

### Creating a data-driven window group

init(_:for:content:)

Creates a data-presenting window group with a text view title.

