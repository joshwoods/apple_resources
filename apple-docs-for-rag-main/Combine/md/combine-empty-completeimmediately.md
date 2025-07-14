

- Combine
- Empty
-  completeImmediately 

Instance Property

# completeImmediately

A Boolean value that indicates whether the publisher immediately sends a completion.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let completeImmediately: Bool
```

## Discussion

If `true`, the publisher finishes immediately after sending a subscription to the subscriber. If `false`, it never completes.

