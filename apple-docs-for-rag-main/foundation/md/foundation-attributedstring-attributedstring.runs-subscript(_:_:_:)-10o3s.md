

- Foundation
- AttributedString
- AttributedString.Runs
-  subscript(\_:\_:\_:) 

Instance Subscript

# subscript(\_:\_:\_:)

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@preconcurrency
subscript(t: KeyPath, u: KeyPath, v: KeyPath) -> AttributedString.Runs.AttributesSlice3 where T : AttributedStringKey, U : AttributedStringKey, V : AttributedStringKey, T.Value : Sendable, U.Value : Sendable, V.Value : Sendable { get }
```

