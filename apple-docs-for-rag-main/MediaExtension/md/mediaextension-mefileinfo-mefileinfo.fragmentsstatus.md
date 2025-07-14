

- MediaExtension
- MEFileInfo
-  MEFileInfo.FragmentsStatus 

Enumeration

# MEFileInfo.FragmentsStatus

An enumeration that describes if a media asset contains or supports fragments.

macOS 14.0+

``` source
enum FragmentsStatus
```

## Overview

For QuickTime movie and ISO files, it indicates the presence of an `mvex` box, which is necessary to signal the possible presence of later `moof` boxes.

## Topics

### File fragment status values

case couldNotContainFragments

The file isn’t extendable by fragments.

case containsFragments

The file is extendable by fragments and contains at least one fragment.

case couldContainButDoesNotContainFragments

The file is extendable by fragments, but doesn’t contain any fragments.

case couldNotContainFragments

The file isn’t extendable by fragments.

case containsFragments

The file is extendable by fragments and contains at least one fragment.

case couldContainButDoesNotContainFragments

The file is extendable by fragments, but doesn’t contain any fragments.

### Initializers

init?(rawValue: Int)

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Inspecting file properties

var duration: CMTime

The duration of the media asset, if available.

var fragmentsStatus: MEFileInfo.FragmentsStatus

Indicates if the media asset contains fragments or is extendable by fragments.

