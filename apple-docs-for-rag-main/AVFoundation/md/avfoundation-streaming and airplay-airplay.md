

- AVFoundation
-  Streaming and AirPlay 

API Collection

# Streaming and AirPlay

Stream content wirelessly to other devices using AirPlay, and handle requests involving FairPlay-protected assets.

## Topics

### Essentials

Supporting AirPlay in your app

Set up your app to use AirPlay to send content wirelessly.

### Route selection

class AVRouteDetector

An object that detects available media playback routes.

### Buffered playback

Implementing simple enhanced buffering for your content

Configure your app for simple enhanced buffering to stream content faster to AirPlay-enabled devices and supported CarPlay vehicles.

Implementing flexible enhanced buffering for your content

Configure your app for flexible enhanced buffering to stream content faster to AirPlay-enabled devices and supported CarPlay vehicles.

Integrating AirPlay for Long-Form Video Apps

Integrate AirPlay features and implement a dedicated external playback experience by preparing the routing system for long-form video playback.

### Resource loading

class AVAssetResourceLoader

An object that mediates resource requests from a URL asset.

protocol AVAssetResourceLoaderDelegate

Methods you can implement to handle resource-loading requests coming from a URL asset.

class AVAssetResourceLoadingRequest

An object that encapsulates information about a resource request from a resource loader object.

class AVAssetResourceRenewalRequest

An object that encapsulates information about a resource request from a resource loader to renew a previously issued request.

class AVAssetResourceLoadingRequestor

An object that contains information about the originator of a resource-loading request.

class AVAssetResourceLoadingDataRequest

An object for requesting data from a resource that an asset resource-loading request references.

class AVAssetResourceLoadingContentInformationRequest

A query for retrieving essential information about a resource that an asset resource-loading request references.

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

func AVSampleBufferAttachContentKey(CMSampleBuffer, AVContentKey, NSErrorPointer) -> Bool

Attaches a content key to a sample buffer for the purpose of content decryption.

## See Also

### Playback

Media playback

Manage the playback of media assets and interstitial content, independent of how you present that content in your interface.

Offline playback and storage

Download streamed content to disk to allow offline playback, and define policies to automatically remove downloaded assets.

Sample buffer playback

Create custom controllers to play and synchronize the timing of sample buffer streams.

