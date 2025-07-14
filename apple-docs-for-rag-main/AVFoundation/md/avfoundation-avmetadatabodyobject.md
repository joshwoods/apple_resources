

- AVFoundation
-  AVMetadataBodyObject 

Class

# AVMetadataBodyObject

An abstract class that defines the interface for a metadata body object.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
class AVMetadataBodyObject
```

## Overview

A metadata body object represents a single detected body in a picture. It’s the base object used to represent bodies, for example AVMetadataHumanBodyObject, AVMetadataDogBodyObject, and AVMetadataCatBodyObject.

## Topics

### Inspecting Metadata

var bodyID: Int

An integer value that defines the unique identifier of an object in a picture.

## Relationships

### Inherits From

- AVMetadataObject

### Inherited By

- AVMetadataCatBodyObject
- AVMetadataDogBodyObject
- AVMetadataHumanBodyObject
- AVMetadataHumanFullBodyObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Bodies

class AVMetadataCatBodyObject

An object representing a single detected cat body in a picture.

class AVMetadataDogBodyObject

An object representing a single detected dog body in a picture.

class AVMetadataHumanBodyObject

An object representing a single detected human body in a picture.

class AVMetadataHumanFullBodyObject

An object that represents a detected human full body in a picture.

