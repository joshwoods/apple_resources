

- HealthKit
- HKQuantitySeriesSampleQueryDescriptor
-  init(predicate:options:) 

Initializer

# init(predicate:options:)

Creates a quantity series query descriptor.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 13.0+visionOSwatchOS 8.5+

``` source
init(
    predicate: HKSamplePredicate,
    options: HKQuantitySeriesSampleQueryDescriptor.Options = []
)
```

## Parameters 

`predicate`  

A predicate that defines the set of series samples that the query returns. For a list of convenience methods for building predicates, see HKQuery.

`options`  

A set of options for the query. For a list of possible values, see HKQuantitySeriesSampleQueryDescriptor.Options.

## See Also

### Creating Series Query Descriptors

struct Options

Options used when querying series data.

