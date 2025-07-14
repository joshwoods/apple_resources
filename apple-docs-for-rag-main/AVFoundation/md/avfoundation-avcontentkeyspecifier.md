

- AVFoundation
-  AVContentKeySpecifier 

Class

# AVContentKeySpecifier

An object that uniquely identifies a content key.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+tvOS 14.5+visionOS 1.0+watchOS 7.4+

``` source
class AVContentKeySpecifier
```

## Topics

### Creating a Specifier

init(forKeySystem: AVContentKeySystem, identifier: Any, options: [String : Any])

Creates a content key specifier.

### Inspecting a Specifier

var identifier: any Sendable

The container and protocol-specific key identifier.

var keySystem: AVContentKeySystem

The key system that generates content keys.

var options: [String : any Sendable]

A dictionary of options with which you initialized the specifier.

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
- Sendable

## See Also

### FairPlay Streaming

class AVContentKeySession

An object that creates and tracks decryption keys for media data.

protocol AVContentKeySessionDelegate

A protocol that handles content key requests.

class AVContentKey

An object that represents the content key decryptor.

class AVContentKeyRequest

An object that encapsulates information about a content decryption key request issued from a content key session object.

class AVPersistableContentKeyRequest

An object that encapsulates information about a persistable content decryption key request issued from a content key session.

class AVContentKeyResponse

An object that encapsulates information about a response to a content decryption key request.

enum AVExternalContentProtectionStatus

Constants that specify whether sufficient protection exists to display the content.

func AVSampleBufferAttachContentKey(CMSampleBuffer, AVContentKey, NSErrorPointer) -> Bool

Attaches a content key to a sample buffer for the purpose of content decryption.

