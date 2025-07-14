

- SwiftUI
- WindowGroup
-  init(id:content:) Deprecated

Initializer

# init(id:content:)

Creates a window group with an identifier.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
init(
    id: String,
    @ViewBuilder content: () -> Content
)
```

Deprecated

Use the initializer which takes an escaping view builder instead.

## Parameters 

`id`  

A string that uniquely identifies the window group. Identifiers must be unique among the window groups in your app.

`content`  

A closure that creates the content for each instance of the group.

## Discussion

The window group uses the given view as a template to form the content of each window in the group.

## See Also

### Identifying a window group

init(_:id:content:)

Creates a window group with a text view title and an identifier.

Deprecated

