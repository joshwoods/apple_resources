

- Combine
- Publishers
- Publishers.MergeMany
-  init(\_:) 

Initializer

# init(\_:)

Creates a publisher created by applying the merge function to an arbitrary number of upstream publishers.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(_ upstream: Upstream...)
```

## Parameters 

`upstream`  

A variadic parameter containing zero or more publishers to merge with this publisher.

## See Also

### Creating a Merge Many Publisher

init&lt;S>(S)

Creates a publisher created by applying the merge function to a sequence of upstream publishers.

