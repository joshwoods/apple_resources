

- SwiftData
-  Query(\_:animation:) 

Macro

# Query(\_:animation:)

Fetches only the subset of the attached model type that satisfy the provided fetch descriptor’s criteria.

SwiftDataSwiftUIiOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@attached(accessor) @attached(peer, names: prefixed(`_`))
macro Query(
    _ descriptor: FetchDescriptor,
    animation: Animation
) where Element : PersistentModel
```

## Parameters 

`descriptor`  

The criteria, sort order, and any additional configuration to use when performing the fetch.

`animation`  

The animation to use when updates to the fetched models trigger user interface changes.

## See Also

### Descriptor-based queries

macro Query&lt;Element>(FetchDescriptor&lt;Element>, transaction: Transaction?)

Fetches only the subset of the attached model type that satisfy the provided fetch descriptor’s criteria.

