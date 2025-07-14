

- SwiftUI
- Link
-  init(destination:label:) 

Initializer

# init(destination:label:)

Creates a control, consisting of a URL and a label, used to navigate to the given URL.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
init(
    destination: URL,
    @ViewBuilder label: () -> Label
)
```

## Parameters 

`destination`  

The URL for the link.

`label`  

A view that describes the destination of URL.

## See Also

### Creating a link

init(_:destination:)

Creates a control, consisting of a URL and a title key, used to navigate to a URL.

