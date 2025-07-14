

- SwiftUI
- WindowGroup
-  init(id:makeContent:) 

Initializer

# init(id:makeContent:)

Creates a window group with an identifier.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
nonisolated
init(
    id: String,
    @ViewBuilder makeContent: @escaping () -> Content
)
```

Available when `Content` conforms to `View`.

## Parameters 

`id`  

A string that uniquely identifies the window group. Identifiers must be unique among the window groups in your app.

`makeContent`  

A closure that creates the content for each instance of the group.

## Discussion

The window group uses the given view as a template to form the content of each window in the group.

