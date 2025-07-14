

- Foundation
- AttributedString
- AttributedString.Runs
- AttributedString.Runs.Run
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@preconcurrency
subscript(_: K.Type) -> K.Value? where K : AttributedStringKey, K.Value : Sendable { get }
```

