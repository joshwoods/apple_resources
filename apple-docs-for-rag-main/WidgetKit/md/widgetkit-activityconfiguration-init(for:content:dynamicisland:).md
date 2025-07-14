

- WidgetKit
- ActivityConfiguration
-  init(for:content:dynamicIsland:) 

Initializer

# init(for:content:dynamicIsland:)

Creates a configuration object for a Live Activity.

iOS 16.1+iPadOS 16.1+

``` source
@MainActor @preconcurrency
init(
    for attributesType: Attributes.Type,
    @ViewBuilder content: @escaping (ActivityViewContext) -> Content,
    dynamicIsland: @escaping (ActivityViewContext) -> DynamicIsland
) where Content : View
```

## Parameters 

`attributesType`  

The type that describes the content of the Live Activity.

`content`  

A closure that creates the view for the Live Activity that appears on the Lock Screen. This view also appears as a banner on the Home Screen of devices that don’t support the Dynamic Island when you alert a person about updated Live Activity content.

`dynamicIsland`  

A closure that builds the Live Activity that appears in the Dynamic Island.

## See Also

### Creating a Live Activity configuration

struct ActivityViewContext

A structure that describes the view context for creating the views of a Live Activity.

