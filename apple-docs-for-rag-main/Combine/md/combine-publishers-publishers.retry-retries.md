

- Combine
- Publishers
- Publishers.Retry
-  retries 

Instance Property

# retries

The maximum number of retry attempts to perform.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
let retries: Int?
```

## Discussion

If `nil`, this publisher attempts to reconnect with the upstream publisher an unlimited number of times.

## See Also

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives elements.

