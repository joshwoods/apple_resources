

- ManagedAppDistribution
- ManagedContentOfferState
-  installing(progress:) 

Type Method

# installing(progress:)

A state indicating install progress.

ManagedAppDistributionSwiftUIiOS 17.2+iPadOS 17.2+

``` source
static func installing(progress: Double?) -> ManagedContentOfferState
```

## Parameters 

`progress`  

The progress of the install from `0.0` to `1.0`. `nil` represents indeterminate progress.

## See Also

### Creating states

static func custom(title: String) -> ManagedContentOfferState

A state with a custom title.

