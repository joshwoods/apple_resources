

- MediaExtension
- MEFormatReaderParseAdditionalFragmentsStatus
-  fragmentsComplete 

Type Property

# fragmentsComplete

Indicates that the format reader can’t receive any more fragments.

macOS 14.0+

``` source
static var fragmentsComplete: MEFormatReaderParseAdditionalFragmentsStatus { get }
```

## Discussion

Additional calls of parseAdditionalFragments(completionHandler:) return an error.

## See Also

### Evaluating a fragment parsing operation

static var sizeIncreased: MEFormatReaderParseAdditionalFragmentsStatus

Indicates that the format reader file size increased.

static var fragmentAdded: MEFormatReaderParseAdditionalFragmentsStatus

Indicates that the format reader received one or more fragments.

