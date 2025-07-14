

- Address Book
-  ABPersonImageFormat Deprecated

Structure

# ABPersonImageFormat

Indicates an image format.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
struct ABPersonImageFormat
```

## Overview

See `Image Format`.

## Topics

### Constants

init(UInt32)

Initializes an image format with an integer value.

init(rawValue: UInt32)

Initializes an image format with a raw integer value.

### Instance Properties

var rawValue: UInt32

The raw value of an image format.

var kABPersonImageFormatOriginalSize: ABPersonImageFormat

The image at its original size and shape.

var kABPersonImageFormatThumbnail: ABPersonImageFormat

The small square thumbnail.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Deprecated

enum ABAuthorizationStatus

Different possible values for the authorization status of an app with respect to address book data.

Deprecated

