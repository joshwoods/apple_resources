

- DeveloperToolsSupport
- Preview
-  init(\_:traits:body:) 

Initializer

# init(\_:traits:body:)

Creates a preview of an NSViewController.

macOS 14.0+

``` source
@MainActor
init(
    _ name: String? = nil,
    traits: PreviewTrait...,
    body: @escaping @MainActor () -> NSViewController
)
```

## Discussion

The `#Preview` macro expands into a declaration that calls this initializer. To create a preview that appears in the canvas, you must use the macro, not call this initializer directly.

