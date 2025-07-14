

- MediaExtension
-  MEFileInfo 

Class

# MEFileInfo

An object that contains file properties from the media asset.

macOS 14.0+

``` source
class MEFileInfo
```

## Topics

### Inspecting file properties

var duration: CMTime

The duration of the media asset, if available.

var fragmentsStatus: MEFileInfo.FragmentsStatus

Indicates if the media asset contains fragments or is extendable by fragments.

enum FragmentsStatus

An enumeration that describes if a media asset contains or supports fragments.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- Sendable

## See Also

### Format readers

protocol MEFormatReader

A protocol that defines the requirements for a format reader, which represents a single media asset.

protocol MEFormatReaderExtension

A protocol that defines a factory to create a new format reader with a byte source.

class MEFormatReaderInstantiationOptions

An object that contains options to pass to a format reader extension.

Format reader property list dictionaries

Include property list dictionaries to describe a format reader and register the formats it supports.

Format reader entitlement

Include an entitlement to indicate your extension is a MediaExtension format reader.

