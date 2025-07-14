

- MediaExtension
-  MEFormatReaderParseAdditionalFragmentsStatus 

Structure

# MEFormatReaderParseAdditionalFragmentsStatus

Informational status flags that the format reader returns after parsing additional fragments.

macOS 14.0+

``` source
struct MEFormatReaderParseAdditionalFragmentsStatus
```

## Topics

### Creating informational status flags

init(rawValue: UInt)

Create a new information status flag for parsing additional fragments.

### Evaluating a fragment parsing operation

static var sizeIncreased: MEFormatReaderParseAdditionalFragmentsStatus

Indicates that the format reader file size increased.

static var fragmentAdded: MEFormatReaderParseAdditionalFragmentsStatus

Indicates that the format reader received one or more fragments.

static var fragmentsComplete: MEFormatReaderParseAdditionalFragmentsStatus

Indicates that the format reader can’t receive any more fragments.

### Default Implementations

Equatable Implementations

OptionSet Implementations

SetAlgebra Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Reading and parsing media assets

func loadFileInfo(completionHandler: (MEFileInfo?, (any Error)?) -> Void)

Loads the file info object with the properties of the media asset.

**Required**

func loadMetadata(completionHandler: ([AVMetadataItem]?, (any Error)?) -> Void)

Loads the array of metadata items from the media asset.

**Required**

func loadTrackReaders(completionHandler: ([any METrackReader]?, (any Error)?) -> Void)

Loads the array of track readers that represent the tracks in the media asset.

**Required**

func parseAdditionalFragments(completionHandler: (MEFormatReaderParseAdditionalFragmentsStatus, (any Error)?) -> Void)

Incorporates additional fragments that the file received after the last time the format reader parsed it.

