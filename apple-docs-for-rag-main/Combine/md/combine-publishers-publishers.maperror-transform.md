

- Combine
- Publishers
- Publishers.MapError
-  transform 

Instance Property

# transform

The closure that converts the upstream failure into a new error.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let transform: (Upstream.Failure) -> Failure
```

## See Also

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

