

- SwiftUI
-  PreviewContext 

Protocol

# PreviewContext

A context type for use with a preview.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
protocol PreviewContext
```

## Topics

### Accessing a preview context

subscript&lt;Key>(Key.Type) -> Key.Value

Returns the context’s value for a key, or a the key’s default value if the context doesn’t define a value for the key.

**Required**

## See Also

### Setting a context

func previewContext&lt;C>(C) -> some View

Declares a context for the preview.

protocol PreviewContextKey

A key type for a preview context.

