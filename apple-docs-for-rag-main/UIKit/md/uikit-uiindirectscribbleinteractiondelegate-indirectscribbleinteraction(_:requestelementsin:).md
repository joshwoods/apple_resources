

- UIKit
- UIIndirectScribbleInteractionDelegate
-  indirectScribbleInteraction(\_:requestElementsIn:) 

Instance Method

# indirectScribbleInteraction(\_:requestElementsIn:)

iOS 15.0+iPadOS 15.0+Mac CatalystvisionOS

``` source
@MainActor
func indirectScribbleInteraction(
    _ interaction: any UIInteraction,
    requestElementsIn rect: CGRect
) async -> [Self.ElementIdentifier]
```

**Required** Default implementation provided.

## Default Implementations

### UIIndirectScribbleInteractionDelegate Implementations

func indirectScribbleInteraction(any UIInteraction, requestElementsIn: CGRect) async -> [Self.ElementIdentifier]

