

- MediaExtension
-  MEFormatReaderInstantiationOptions 

Class

# MEFormatReaderInstantiationOptions

An object that contains options to pass to a format reader extension.

macOS 14.0+

``` source
class MEFormatReaderInstantiationOptions
```

## Overview

This object is mutable with options set through instance properties.

## Topics

### Inspecting format reader extension options

var allowIncrementalFragmentParsing: Bool

Enables support for parsing additional fragments.

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

class MEFileInfo

An object that contains file properties from the media asset.

Format reader property list dictionaries

Include property list dictionaries to describe a format reader and register the formats it supports.

Format reader entitlement

Include an entitlement to indicate your extension is a MediaExtension format reader.

