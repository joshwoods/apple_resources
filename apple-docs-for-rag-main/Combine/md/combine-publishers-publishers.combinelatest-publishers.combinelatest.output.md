

- Combine
- Publishers
- Publishers.CombineLatest
-  Publishers.CombineLatest.Output 

Type Alias

# Publishers.CombineLatest.Output

The kind of values published by this publisher.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
typealias Output = (A.Output, B.Output)
```

## Discussion

This publisher produces two-element tuples of the upstream publishers’ output types.

## See Also

### Declaring Publisher Topography

typealias Failure

The kind of errors this publisher might publish.

