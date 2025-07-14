

- FSKit
- FSVolume
-  FSVolume.SupportedCapabilities 

Class

# FSVolume.SupportedCapabilities

A type that represents capabillities supported by a volume, such as hard and symbolic links, journaling, and large file sizes.

macOS 15.4+

``` source
class SupportedCapabilities
```

## Topics

### Declaring identifier capabilities

var supportsPersistentObjectIDs: Bool

A Boolean property that indicates whether the volume supports persistent object identifiers and can look up file system objects by their IDs.

var supports64BitObjectIDs: Bool

A Boolean property that indicates whether the volume supports 64-bit object IDs.

var supportsDocumentID: Bool

A Boolean property that indicates whether the volume supports document IDs for document revisions.

### Declaring linking capabilities

var supportsSymbolicLinks: Bool

A Boolean property that indicates whether the volume supports symbolic links.

var supportsHardLinks: Bool

A Boolean property that indicates whether the volume supports hard links.

### Declaring journaling capabilities

var supportsJournal: Bool

A Boolean property that indicates whether the volume supports a journal used to speed recovery in case of unplanned restart, such as a power outage or crash.

var supportsActiveJournal: Bool

A Boolean property that indicates whether the volume currently uses a journal for speeding recovery after an unplanned shutdown.

### Declaring root capabilites

var doesNotSupportRootTimes: Bool

A Boolan property that indicates the volume doesn’t store reliable times for the root directory.

### Declaring file capabilities

var supportsSparseFiles: Bool

A Boolean property that indicates whether the volume supports sparse files.

var supportsZeroRuns: Bool

A Boolean property that indicates whether the volume supports zero runs

var supportsFastStatFS: Bool

A Boolean property that indicates whether the volume supports fast results when fetching file system statistics.

var supports2TBFiles: Bool

A Boolean property that indicates whether the volume supports file sizes larger than 4GB, and potentially up to 2TB.

var supportsOpenDenyModes: Bool

A Boolean property that indicates whether the volume supports open deny modes.

var supportsHiddenFiles: Bool

A Boolean property that indicates whether the volume supports hidden files.

var doesNotSupportImmutableFiles: Bool

A Boolean property that indicates the volume doesn’t support immutable files.

var doesNotSupportSettingFilePermissions: Bool

A Boolean property that indicates the volume doesn’t set file permissions.

### Declaring volume capabilities

var supportsSharedSpace: Bool

A Boolean property that indicates whether the volume supports multiple logical file systems that share space in a single “partition.”

var supportsVolumeGroups: Bool

A Boolean property that indicates whether the volume supports volume groups.

var doesNotSupportVolumeSizes: Bool

A Boolean property that indicates the volume doesn’t support certain volume size reports.

### Working with case sensitivity

var caseFormat: FSVolume.CaseFormat

A value that indicates the volume’s support for case sensitivity.

enum CaseFormat

An enumeration of case-sensitivity support types.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Inspecting volume properties

var supportedVolumeCapabilities: FSVolume.SupportedCapabilities

A property that provides the supported capabilities of the volume.

**Required**

var volumeStatistics: FSStatFSResult

A property that provides up-to-date statistics of the volume.

**Required**

class FSStatFSResult

A type used to report a volume’s statistics.

