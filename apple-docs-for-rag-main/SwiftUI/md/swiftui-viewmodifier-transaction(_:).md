

- SwiftUI
- ViewModifier
-  transaction(\_:) 

Instance Method

# transaction(\_:)

Returns a new version of the modifier that will apply the transaction mutation function `transform` to all transactions within the modifier.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func transaction(_ transform: @escaping (inout Transaction) -> Void) -> some ViewModifier
```

