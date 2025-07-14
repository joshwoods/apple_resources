

- ShazamKit
-  SHSignatureGenerator 

Class

# SHSignatureGenerator

An object for converting audio data into a signature.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class SHSignatureGenerator
```

## Mentioned in 

Generating a signature from an audio buffer

## Overview

Create both reference and query signatures using this class.

## Topics

### Generating a signature from audio

func append(AVAudioPCMBuffer, at: AVAudioTime?) throws

Adds audio to the generator.

func signature() -> SHSignature

Converts the audio buffer into a signature.

Generating a signature from an audio buffer

Create a signature from an audio file or the microphone for a reference track in a custom catalog, or for matching tracks in a catalog.

### Generate a signature from assets

class func generateSignature(from: AVAsset, completionHandler: (SHSignature?, (any Error)?) -> Void)

Creates a signature with the asset you specify.

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

### Create a signature from audio

class SHSignature

An object that contains the opaque data and other information for a signature.

