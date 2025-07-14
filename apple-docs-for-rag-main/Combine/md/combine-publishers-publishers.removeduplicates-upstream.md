

- Combine
- Publishers
- Publishers.RemoveDuplicates
-  upstream 

Instance Property

# upstream

The publisher from which this publisher receives elements.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let upstream: Upstream
```

## See Also

### Inspecting Publisher Properties

let predicate: (Publishers.RemoveDuplicates&lt;Upstream>.Output, Publishers.RemoveDuplicates&lt;Upstream>.Output) -> Bool

The predicate closure used to evaluate whether two elements are duplicates.

