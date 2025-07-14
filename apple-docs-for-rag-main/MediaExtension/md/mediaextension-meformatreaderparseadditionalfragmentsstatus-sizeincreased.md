

- MediaExtension
- MEFormatReaderParseAdditionalFragmentsStatus
-  sizeIncreased 

Type Property

# sizeIncreased

Indicates that the format reader file size increased.

macOS 14.0+

``` source
static var sizeIncreased: MEFormatReaderParseAdditionalFragmentsStatus { get }
```

## See Also

### Evaluating a fragment parsing operation

static var fragmentAdded: MEFormatReaderParseAdditionalFragmentsStatus

Indicates that the format reader received one or more fragments.

static var fragmentsComplete: MEFormatReaderParseAdditionalFragmentsStatus

Indicates that the format reader can’t receive any more fragments.

