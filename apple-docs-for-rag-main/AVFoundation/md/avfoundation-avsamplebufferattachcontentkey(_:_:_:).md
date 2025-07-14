

- AVFoundation
-  AVSampleBufferAttachContentKey(\_:\_:\_:) 

Function

# AVSampleBufferAttachContentKey(\_:\_:\_:)

Attaches a content key to a sample buffer for the purpose of content decryption.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+tvOS 14.5+visionOS 1.0+watchOS 7.4+

``` source
func AVSampleBufferAttachContentKey(
    _ sbuf: CMSampleBuffer,
    _ contentKey: AVContentKey,
    _ outError: NSErrorPointer
) -> Bool
```

## Parameters 

`sbuf`  

The sample buffer to which to attach the content key.

`contentKey`  

The content key to attach.

`outError`  

An error pointer. If a failure occurs, the system sets the pointer to an error object that describes the details of the failure.

## Return Value

A Boolean value that indicates whether the attachment is successful.

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

class AVPersistableContentKeyRequest

An object that encapsulates information about a persistable content decryption key request issued from a content key session.

class AVContentKeyResponse

An object that encapsulates information about a response to a content decryption key request.

enum AVExternalContentProtectionStatus

Constants that specify whether sufficient protection exists to display the content.

