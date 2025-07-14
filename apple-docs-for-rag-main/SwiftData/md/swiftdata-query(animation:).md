

- SwiftData
-  Query(animation:) 

Macro

# Query(animation:)

Fetches all instances of the attached model type, using the specified animation to animate any subsequent changes.

SwiftDataSwiftUIiOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@attached(accessor) @attached(peer, names: prefixed(`_`))
macro Query(animation: Animation)
```

## Parameters 

`animation`  

The animation to use when updates to the fetched models trigger user interface changes.

## See Also

### Basic queries

macro Query(transaction: Transaction)

Fetches all instances of the attached model type, using the specified transaction to animate any subsequent changes.

