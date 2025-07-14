

- ShazamKit
-  SHSignature 

Class

# SHSignature

An object that contains the opaque data and other information for a signature.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class SHSignature
```

## Overview

Save your signature to a file and share it with others by writing the data to a file. You can use the saved signatures of reference recordings to populate a custom catalog.

Check whether your captured query signature is long enough to search for a match by comparing duration to the minimumQuerySignatureDuration and maximumQuerySignatureDuration of a catalog.

## Topics

### Creating a signature object

init(dataRepresentation: Data) throws

Creates a signature object from raw data.

### Reading signature information

var dataRepresentation: Data

The raw data for the signature.

var duration: TimeInterval

The duration of the audio you use to generate the signature.

### Getting the content type

static var shazamSignature: UTType { get }

A type that represents a signature.

### Structures

struct Slices

### Instance Methods

func slices(from: TimeInterval, duration: TimeInterval, stride: TimeInterval?) throws -> SHSignature.Slices

Returns a sequence of signatures of the specified duration from a starting value, stepping by the stride.

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
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Create a signature from audio

class SHSignatureGenerator

An object for converting audio data into a signature.

