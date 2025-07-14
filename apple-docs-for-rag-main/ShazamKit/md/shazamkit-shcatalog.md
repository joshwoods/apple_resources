

- ShazamKit
-  SHCatalog 

Class

# SHCatalog

An abstract base class for storing reference signatures and their associated metadata.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class SHCatalog
```

## Overview

This is the base class of your custom catalog.

## Topics

### Accessing catalog properties

var maximumQuerySignatureDuration: TimeInterval

The maximum duration of a query signature that you use to match reference signatures in the catalog.

var minimumQuerySignatureDuration: TimeInterval

The minimum duration of a query signature that you use to match reference signatures in the catalog.

## Relationships

### Inherits From

- NSObject

### Inherited By

- SHCustomCatalog

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Create a custom audio catalog

Building a Custom Catalog and Matching Audio

Display lesson content that’s synchronized to a learning video by matching the audio to a custom reference signature and associated metadata.

ShazamKit Dance Finder with Managed Session

Find a video of dance moves for a specific song by matching the audio to a custom catalog, and show a history of recognized songs.

class SHCustomCatalog

An object for storing the reference signatures for custom audio recordings and their associated metadata.

