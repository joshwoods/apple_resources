

- Foundation
- AttributedString
- AttributedString.Runs
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@preconcurrency
subscript(t: T.Type) -> AttributedString.Runs.AttributesSlice1 where T : AttributedStringKey, T.Value : Sendable { get }
```

