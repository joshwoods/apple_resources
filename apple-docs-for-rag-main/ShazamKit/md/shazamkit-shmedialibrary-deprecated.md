

- ShazamKit
-  SHMediaLibrary Deprecated

Class

# SHMediaLibrary

An object that represents the user’s Shazam library.

iOS 15.0–18.0DeprecatediPadOS 15.0–18.0DeprecatedMac Catalyst 15.0–18.0DeprecatedmacOS 12.0–15.0DeprecatedtvOS 15.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 8.0–11.0Deprecated

``` source
class SHMediaLibrary
```

Deprecated

Use SHLibrary instead.

## Overview

Use `SHMediaLibrary` to add matched songs from the Shazam catalog to the user’s Shazam library.

Note

There’s no system permission necessary to write to the user’s Shazam library. Consider requesting permission from the user before adding songs to the library.

## Topics

### Adding a matched song to the library

class var `default`: SHMediaLibrary

An instance of the user’s default Shazam library.

func add([SHMediaItem], completionHandler: ((any Error)?) -> Void)

Adds an array of songs to the user’s Shazam library.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Update the user’s Shazam library

class SHLibrary

An object that represents a user’s synced Shazam library.

