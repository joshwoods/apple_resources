

- Combine
- Publishers
- Publishers.Zip3
-  Publishers.Zip3.Output 

Type Alias

# Publishers.Zip3.Output

The kind of values published by this publisher.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
typealias Output = (A.Output, B.Output, C.Output)
```

## Discussion

This publisher produces three-element tuples, whose members’ types correspond to the types produced by the upstream publishers.

## See Also

### Declaring Publisher Topography

typealias Failure

The kind of errors this publisher might publish.

