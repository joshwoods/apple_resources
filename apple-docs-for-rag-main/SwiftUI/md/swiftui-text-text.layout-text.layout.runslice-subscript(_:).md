

- SwiftUI
- Text
- Text.Layout
- Text.Layout.RunSlice
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

The custom attribute of type `T` associated with the run of glyphs, or nil.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
subscript(key: T.Type) -> T? where T : TextAttribute { get }
```

