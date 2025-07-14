

- Combine
- Publishers
- Publishers.TryCompactMap
-  transform 

Instance Property

# transform

An error-throwing closure that receives values from the upstream publisher and returns optional values.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let transform: (Upstream.Output) throws -> Output?
```

## Discussion

If this closure throws an error, the publisher fails.

## See Also

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

