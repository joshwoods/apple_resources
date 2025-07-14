

- SwiftUI
- PreviewContext
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Returns the context’s value for a key, or a the key’s default value if the context doesn’t define a value for the key.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
subscript(key: Key.Type) -> Key.Value where Key : PreviewContextKey { get }
```

**Required**

