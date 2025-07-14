

- SwiftUI
- PreviewModifier
-  body(content:context:) 

Instance Method

# body(content:context:)

Modify a preview by applying the shared context.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@ViewBuilder @MainActor
func body(
    content: Self.Content,
    context: Self.Context
) -> Self.Body
```

**Required**

## Parameters 

`content`  

A proxy for the preview being modified.

`context`  

The shared context to apply.

