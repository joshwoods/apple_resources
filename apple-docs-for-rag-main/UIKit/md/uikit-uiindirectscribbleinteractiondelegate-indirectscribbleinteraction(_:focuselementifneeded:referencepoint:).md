

- UIKit
- UIIndirectScribbleInteractionDelegate
-  indirectScribbleInteraction(\_:focusElementIfNeeded:referencePoint:) 

Instance Method

# indirectScribbleInteraction(\_:focusElementIfNeeded:referencePoint:)

iOS 15.0+iPadOS 15.0+Mac CatalystvisionOS

``` source
@MainActor
func indirectScribbleInteraction(
    _ interaction: any UIInteraction,
    focusElementIfNeeded elementIdentifier: Self.ElementIdentifier,
    referencePoint focusReferencePoint: CGPoint
) async -> (any UIResponder & UITextInput)?
```

**Required** Default implementation provided.

## Default Implementations

### UIIndirectScribbleInteractionDelegate Implementations

func indirectScribbleInteraction(any UIInteraction, focusElementIfNeeded: Self.ElementIdentifier, referencePoint: CGPoint) async -> (any UIResponder &amp; UITextInput)?

