

- SwiftUI
- PreviewModifier
-  makeSharedContext() 

Type Method

# makeSharedContext()

Create shared context to apply to previews. The context returned here will be cached and passed into the `body` method for every preview that applies a modifier of this type.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@MainActor
static func makeSharedContext() async throws -> Self.Context
```

**Required** Default implementation provided.

## Default Implementations

### PreviewModifier Implementations

static func makeSharedContext() async throws -> Self.Context

Create shared context to apply to previews. The context returned here will be cached and passed into the `body` method for every preview that applies a modifier of this type.

