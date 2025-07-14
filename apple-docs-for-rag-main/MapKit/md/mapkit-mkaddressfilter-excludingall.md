

- MapKit
- MKAddressFilter
-  excludingAll 

Type Property

# excludingAll

A list of categories to exclude from a search.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
class var excludingAll: MKAddressFilter { get }
```

## See Also

### Filtering results

struct Options

A structure that contains options for filtering results in a search.

class var includingAll: MKAddressFilter

A list of categories to include in a search.

func excludes(MKAddressFilter.Options) -> Bool

Indicates whether options are excluded from filtering.

func includes(MKAddressFilter.Options) -> Bool

Indicates whether options are included for filtering.

