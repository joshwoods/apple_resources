

- SwiftUI
-  PreviewModifier 

Protocol

# PreviewModifier

A type that defines an environment in which previews can appear.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@MainActor
protocol PreviewModifier
```

## Overview

Conforming types can define shared contexts that will be cached by the preview system, then reused across participating previews. For example, you might create a model container here and populate it with sample data; in your `body` method you would then apply it to the preview using the `.modelContainer` view modifier.

```
struct SampleData: PreviewModifier {
    static func makeSharedContext() throws -> ModelContainer {
        let container = try ModelContainer(for: Snack.self)
        container.mainContext.insert(Snack.potatoChips)
        return container
    }

    func body(content: Content, context: ModelContainer) -> some View {
        content.modelContainer(context)
    }
 }
```

Use the `.modifier` preview trait to attach modifiers to a preview.

```
#Preview(traits: .modifier(SampleData())) {
    @Previewable @Query var snacks: [Snack]
    return SnackView(snack: snacks.first!)
}
```

## Topics

### Associated Types

associatedtype Body : View

**Required**

associatedtype Context = Void

**Required**

### Instance Methods

func body(content: Self.Content, context: Self.Context) -> Self.Body

Modify a preview by applying the shared context.

**Required**

### Type Aliases

typealias Content

The type-erased content of a preview.

### Type Methods

static func makeSharedContext() async throws -> Self.Context

Create shared context to apply to previews. The context returned here will be cached and passed into the `body` method for every preview that applies a modifier of this type.

**Required** Default implementation provided.

## See Also

### Defining a preview

macro Previewable()

Tag allowing a dynamic property to appear inline in a preview.

protocol PreviewProvider

A type that produces view previews in Xcode.

enum PreviewPlatform

Platforms that can run the preview.

func previewDisplayName(String?) -> some View

Sets a user visible name to show in the canvas for a preview.

struct PreviewModifierContent

The type-erased content of a preview.

