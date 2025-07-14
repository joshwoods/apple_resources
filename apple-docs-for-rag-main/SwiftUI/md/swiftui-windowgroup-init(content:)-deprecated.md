

- SwiftUI
- WindowGroup
-  init(content:) Deprecated

Initializer

# init(content:)

Creates a window group.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
init(@ViewBuilder content: () -> Content)
```

Deprecated

Use the initializer which takes an escaping view builder instead.

## Parameters 

`content`  

A closure that creates the content for each instance of the group.

## Discussion

The window group uses the given view as a template to form the content of each window in the group.

## See Also

### Creating a window group

init(_:content:)

Creates a window group with a text view title.

Deprecated

