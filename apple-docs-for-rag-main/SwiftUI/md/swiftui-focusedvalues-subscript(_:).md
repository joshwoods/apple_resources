

- SwiftUI
- FocusedValues
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Reads and writes values associated with a given focused value key.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
subscript(key: Key.Type) -> Key.Value? where Key : FocusedValueKey { get set }
```

