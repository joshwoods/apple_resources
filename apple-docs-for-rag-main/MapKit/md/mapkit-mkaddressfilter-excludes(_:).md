

- MapKit
- MKAddressFilter
-  excludes(\_:) 

Instance Method

# excludes(\_:)

Indicates whether options are excluded from filtering.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func excludes(_ options: MKAddressFilter.Options) -> Bool
```

## Parameters 

`options`  

The filters to check for exclusion.

## Return Value

Returns `true` if the passed options are excluded from the filtering options; otherwise, `false`.

## Discussion

A filter includes or excludes a set of filter options. Use this method to query the filter instance for one or more options.

```
let filter = MKAddressFilter(including: [.locality,  .subLocality])
let result = filter.excludes(.postalCode)
```

The method returns `true` because `filter` doesn’t include PostalCode.

## See Also

### Filtering results

struct Options

A structure that contains options for filtering results in a search.

class var excludingAll: MKAddressFilter

A list of categories to exclude from a search.

class var includingAll: MKAddressFilter

A list of categories to include in a search.

func includes(MKAddressFilter.Options) -> Bool

Indicates whether options are included for filtering.

