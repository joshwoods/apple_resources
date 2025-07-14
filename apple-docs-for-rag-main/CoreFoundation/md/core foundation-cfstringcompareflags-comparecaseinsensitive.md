

- Core Foundation
- CFStringCompareFlags
-  compareCaseInsensitive 

Type Property

# compareCaseInsensitive

Specifies that the comparison should ignore differences in case between alphabetical characters.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static var compareCaseInsensitive: CFStringCompareFlags { get }
```

## See Also

### Constants

static var compareBackwards: CFStringCompareFlags

Specifies that the comparison should start at the last elements of the entities being compared (for example, strings or arrays).

static var compareAnchored: CFStringCompareFlags

Performs searching only on characters at the beginning or end of the range.

static var compareNonliteral: CFStringCompareFlags

Specifies that loose equivalence is acceptable, especially as pertains to diacritical marks.

static var compareLocalized: CFStringCompareFlags

Specifies that the comparison should take into account differences related to locale, such as the thousands separator character.

static var compareNumerically: CFStringCompareFlags

Specifies that represented numeric values should be used as the basis for comparison and not the actual character values.

static var compareDiacriticInsensitive: CFStringCompareFlags

Specifies that the comparison should ignore diacritic markers.

static var compareWidthInsensitive: CFStringCompareFlags

Specifies that the comparison should ignore width differences.

static var compareForcedOrdering: CFStringCompareFlags

Specifies that the comparison is forced to return either `kCFCompareLessThan` or `kCFCompareGreaterThan` if the strings are equivalent but not strictly equal.

