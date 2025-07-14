

- AVFoundation
-  Offline playback and storage 

API Collection

# Offline playback and storage

Download streamed content to disk to allow offline playback, and define policies to automatically remove downloaded assets.

## Topics

### Asset downloading

Using AVFoundation to play and persist HTTP Live Streams

Play HTTP Live Streams and persist streams on disk for offline playback using AVFoundation.

class AVAssetDownloadURLSession

A URL session that creates and executes asset download tasks.

class AVAssetDownloadTask

A session used to download HTTP Live Streaming assets.

class AVAggregateAssetDownloadTask

A task that downloads multiple media selections for an asset.

### Offline storage management

class AVAssetDownloadStorageManager

An object that manages policies to automatically purge downloaded assets.

class AVAssetDownloadStorageManagementPolicy

An object that defines a policy to automatically manage the storage of downloaded assets.

class AVMutableAssetDownloadStorageManagementPolicy

A mutable object that you use to create a new storage management policy.

### Cache monitoring

class AVAssetCache

An object that you use to inspect locally cached media data.

## See Also

### Playback

Media playback

Manage the playback of media assets and interstitial content, independent of how you present that content in your interface.

Streaming and AirPlay

Stream content wirelessly to other devices using AirPlay, and handle requests involving FairPlay-protected assets.

Sample buffer playback

Create custom controllers to play and synchronize the timing of sample buffer streams.

