

- AVFoundation
-  AVPersistableContentKeyRequest 

Class

# AVPersistableContentKeyRequest

An object that encapsulates information about a persistable content decryption key request issued from a content key session.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.1+macOS 10.15+tvOS 10.2+visionOS 1.0+watchOS 7.0+

``` source
class AVPersistableContentKeyRequest
```

## Overview

This class allows clients to create and use persistable content keys.

## Topics

### Requesting Persistable Content Key Data

func persistableContentKey(fromKeyVendorResponse: Data, options: [String : Any]?) throws -> Data

Creates a persistable content key from the content key context data.

## Relationships

### Inherits From

- AVContentKeyRequest

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### FairPlay Streaming

class AVContentKeySession

An object that creates and tracks decryption keys for media data.

protocol AVContentKeySessionDelegate

A protocol that handles content key requests.

class AVContentKey

An object that represents the content key decryptor.

class AVContentKeySpecifier

An object that uniquely identifies a content key.

class AVContentKeyRequest

An object that encapsulates information about a content decryption key request issued from a content key session object.

class AVContentKeyResponse

An object that encapsulates information about a response to a content decryption key request.

enum AVExternalContentProtectionStatus

Constants that specify whether sufficient protection exists to display the content.

func AVSampleBufferAttachContentKey(CMSampleBuffer, AVContentKey, NSErrorPointer) -> Bool

Attaches a content key to a sample buffer for the purpose of content decryption.

