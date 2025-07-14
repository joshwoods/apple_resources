

- Foundation
- ScopedAttributeContainer
-  subscript(dynamicMember:) 

Instance Subscript

# subscript(dynamicMember:)

Returns the value of the attribute that the specified key path indicates.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@preconcurrency
subscript(dynamicMember keyPath: KeyPath) -> T.Value? where T : AttributedStringKey, T.Value : Sendable { get set }
```

