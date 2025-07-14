

- SwiftData
- Query
-  wrappedValue 

Instance Property

# wrappedValue

The most recent fetched result from the Query.

SwiftDataSwiftUIiOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@MainActor @preconcurrency
var wrappedValue: Result { get }
```

## Discussion

Note

When an fetch error occurs, `wrappedValue` retains results from the last successful fetch. Its value will update once a new fetch succeeds.

