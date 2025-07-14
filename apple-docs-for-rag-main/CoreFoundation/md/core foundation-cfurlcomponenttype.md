

- Core Foundation
-  CFURLComponentType 

Enumeration

# CFURLComponentType

The types of components in a URL.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CFURLComponentType
```

## Overview

These constants are used by the CFURLGetByteRangeForComponent(_:_:_:) function.

## Topics

### Constants

case scheme

The URL’s scheme.

case netLocation

The URL’s network location.

case path

The URL’s path component.

case resourceSpecifier

The URL’s resource specifier.

case user

The URL’s user.

case password

The user’s password.

case userInfo

The user’s information.

case host

The URL’s host.

case port

The URL’s port.

case parameterString

The URL’s parameter string.

case query

The URL’s query.

case fragment

The URL’s fragment.

### Initializers

init?(rawValue: CFIndex)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Miscellaneous

enum CFURLPathStyle

Options you can use to determine how CFURL functions parse a file system path name.

