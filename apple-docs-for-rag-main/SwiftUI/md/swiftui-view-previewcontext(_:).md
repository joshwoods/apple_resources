

- SwiftUI
- View
-  previewContext(\_:) 

Instance Method

# previewContext(\_:)

Declares a context for the preview.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
nonisolated
func previewContext(_ value: C) -> some View where C : PreviewContext
```

## Parameters 

`value`  

The context for the preview; the default is `nil`.

## See Also

### Setting a context

protocol PreviewContext

A context type for use with a preview.

protocol PreviewContextKey

A key type for a preview context.

